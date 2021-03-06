# WazuhMonitoringDoc

**On Agent :**

The package for macOS is suitable for macOS Sierra or greater. The macOS agent can be downloaded from packages list. You can install it by using the command line or following the GUI steps:

https://documentation.wazuh.com/3.10/installation-guide/packages-list/index.html#packages

Use the GUI to install it.

The registration service requires an SSL certificate on the manager in order to work. This certificate will be automatically generated by the package during the installation if the openssl package is installed. This certificate is stored in */var/ossec/etc/sslmanager.cert*.

If you already have a certificate, you can use them just by copying them into the same path:

````
# cp <ssl_cert> /var/ossec/etc/sslmanager.cert
# cp <ssl_key> /var/ossec/etc/sslmanager.key
````

Otherwise, you can create a self-signed certificate using the following command:

````
# openssl req -x509 -batch -nodes -days 365 -newkey rsa:4096 -out /var/ossec/etc/sslmanager.cert -keyout /var/ossec/etc/sslmanager.key
````

Open a terminal in your MacOS X agent host as root user. After that, you can register the Agent using agent-auth as follows:

On the agent, run the agent-auth program, using the manager’s IP address.

````
# /Library/Ossec/bin/agent-auth -m <MANAGER_IP_ADDRESS>
````

Edit the Wazuh agent configuration to add the Wazuh server IP address.
In the file /Library/Ossec/etc/ossec.conf, in the client server section, change the MANAGER_IP value to the Wazuh server address:

```
<client>
  <server>
    <address>MANAGER_IP</address>
    ...
  </server>
</client>

```

Start the agent.

````
# /Library/Ossec/bin/ossec-control start
````