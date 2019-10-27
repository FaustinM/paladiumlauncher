# Documentation du projet

Ce dossier contient toute la documentation du projet et l'organisation du projet

## Principes généraux

Le projet est le launcher du serveur Paladium. Actuellement le launcher est basé sur [Electron](https://electron.js.org) et le launcher de [Westeros](https://github.com/WesterosCraft/ElectronLauncher). Le système de template est [EJS](ejs.org).

## Comment le launcher démarre ?

### 1) [index.js](https://github.com/Chaika9/paladiumlauncher/blob/master/index.js)

Ce fichier est le premier fichier lancé, il crée une nouvelle app puis après lancement de l'auto update, il ouvre preloader.js

###  Backend
#### 2) [app/assets/js/preloader.js](https://github.com/Chaika9/paladiumlauncher/blob/master/app/assets/js/preloader.js)

Ce fichier se charge de mettre la première ligne de log et de nettoyer le dossier temporaire.

#### 3) [app/assets/js/configmanager.js](https://github.com/Chaika9/paladiumlauncher/blob/master/app/assets/js/configmanager.js)

Configmanager se charge de créer le fichier config.json si il n'est pas crée ou de le vérifier et le charger dans le cas contraire

###  Frontend
#### 1) [app/app.ejs](https://github.com/Chaika9/paladiumlauncher/blob/master/app/app.ejs)

App.ejs est le premier fichier du frontend, il appel swinger.js et swingerinterface.js.

#### 2) [app/js/scripts/swinger.js](https://github.com/Chaika9/paladiumlauncher/blob/master/app/assets/js/scripts/swinger.js)

Swinger.js se charge de charger le fichier de distribution et d'informer si il y a une mise à jour. Ainsi que d'autres éléments comme :

* L'épée animée 
#### 3) 
