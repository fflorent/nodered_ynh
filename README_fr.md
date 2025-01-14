# Node-RED pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/nodered.svg)](https://dash.yunohost.org/appci/app/nodered) ![](https://ci-apps.yunohost.org/ci/badges/nodered.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/nodered.maintain.svg)  
[![Installer Node-RED avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=nodered)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer Node-RED rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

Node-RED est un outil de programmation pour connecter des appareils, API, et des services en ligne en de nouvelles et intéressantes façons.

Il propose un éditeur accessible dans le navigateur, qui facilite l'ébauche de flux qui connectent ensemble la grande variété de nœuds disponibles dans sa palette. Ces flux sont ensuite activables et déployables en un clic.

### Fonctionnalités

- Edition de flux dans le navigateur
- Déploiement des flux en un clic
- Plus de 225 000 modules disponibles
- Fonctions personnalisées en JavaScript


**Version incluse :** 2.1.4~ynh1



## Captures d'écran

![](./doc/screenshots/screenshot.jpg)

## Avertissements / informations importantes

Le système de permissions de YunoHost permet de paramétrer les accès à Node-RED :
* la permission `main` protège `/admin`, l'éditeur de flux. L'administrateur est sélectionné pendant l'installation ;
* la permisison `ui` protège `/ui`, le tableau de bord permettant de donner une interface graphique aux flux. L'accès public est défini lors de l'installation ;
* la permission `endpoints` protège `/`, pour notamment les points d'entrée de type API. L'accès public est défini lors de l'installation.

Si vous avez mis à jour Node-RED au-delà de la version 2, vérifiez que ces permissions vous conviennent dans votre panneau d'administration de YunoHost.

## Documentations et ressources

* Site officiel de l'app : https://nodered.org
* Documentation officielle utilisateur : https://nodered.org/docs/
* Dépôt de code officiel de l'app : https://github.com/node-red/node-red
* Documentation YunoHost pour cette app : https://yunohost.org/app_nodered
* Signaler un bug : https://github.com/YunoHost-Apps/nodered_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/nodered_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/nodered_ynh/tree/testing --debug
ou
sudo yunohost app upgrade nodered -u https://github.com/YunoHost-Apps/nodered_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps