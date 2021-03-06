# Installation de Proxmox

Tutoriel réalisé par l'équipe workstation 2019-2020.

## Prérequis

1. Serveur Jarvis.
2. ISO [Proxmox](https://www.proxmox.com/en/downloads).
3. Clé USB.
4. [balenaEtcher](https://www.balena.io/etcher).

## Création de la clé USB

1. Insérez votre clé USB.

2. Exécutez balenaEtcher.

![Exécutez balenaEtcher.](https://raw.githubusercontent.com/WarTey/workstation/master/img/etcher/capture_1.png)

3. Sélectionnez l'ISO Proxmox.

![Sélectionnez l'ISO Proxmox.](https://raw.githubusercontent.com/WarTey/workstation/master/img/etcher/capture_2.png)

4. Cliquez sur 'Flash!' et attendez la fin du processus.

![Cliquez sur 'Flash!' et attendez la fin du processus.](https://raw.githubusercontent.com/WarTey/workstation/master/img/etcher/capture_3.png)

5. Vous pouvez maintenant éjecter la clé USB et procéder à l'installation de Proxmox.

![Vous pouvez maintenant éjecter la clé USB et procéder à l'installation de Proxmox.](https://raw.githubusercontent.com/WarTey/workstation/master/img/etcher/capture_4.png)

## Installation de Proxmox sur le serveur Jarvis

1. Branchez la clé USB à l'arrière du serveur.

2. Au démarrage du serveur, appuyez sur la touche 'F11' et sélectionnez 'Generic USB Boot' pour démarrer sur l'IOS Proxmox.

3. Une fois que la page ci-dessous apparaît, sélectionnez 'Install Proxmox VE'.

![Une fois que cette page apparaît, sélectionnez 'Install Proxmox VE'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_1.png)

4. Cliquez sur 'I agree'.

![Cliquez sur 'I agree'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_2.png)

5. Cliquez sur 'Next'.

![Cliquez sur 'Next'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_3.png)

6. Saisissez 'France' dans le champ 'Country' puis cliquez sur 'Next'.

![Saisissez 'France' dans le champ 'Country' puis cliquez sur 'Next'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_4.png)

7. Choisissez un mot de passe fort et saisissez le dans les champs 'Password' et 'Confirm'. Puis entrez une adresse mail dans le champ suivant et cliquez sur 'Next'.

![Choisissez un mot de passe fort et saisissez le dans les champs 'Password' et 'Confirm'. Puis entrez une adresse mail dans le champ suivant et cliquez sur 'Next'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_5.png)

8. Cliquez sur 'Next'.

![Cliquez sur 'Next'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_6.png)

9. Cliquez sur 'Install' et attendez la fin de l'installation.

![Cliquez sur 'Install' et attendez la fin de l'installation.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_7.png)

![Cliquez sur 'Install' et attendez la fin de l'installation.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_8.png)

10. Cliquez sur 'Reboot'.

![Cliquez sur 'Reboot'.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_9.png)

11. Vous pouvez maintenant vous connecter sur le serveur ou depuis une page web en saisissant l'adresse indiquait.

![Vous pouvez maintenant vous connecter sur le serveur ou depuis une page web en saisissant l'adresse indiquait.](https://raw.githubusercontent.com/WarTey/workstation/master/img/proxmox/capture_10.png)

12. Par défaut, le nom d'utilisateur est 'root'.

13. Vous pouvez maintenant passer à la configuration de Proxmox et à l'installation de l'active directory.