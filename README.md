# Application de Chat Node.js

Une application de démonstration de chat simple construite avec [Node.js](https://nodejs.org/), [Express.js](https://expressjs.com/) et [Socket.io](https://socket.io/).

## Démo

https://owan-nodejs-chat-app.herokuapp.com

## Prérequis

Pour configurer et exécuter le projet en développement / test local, vous devrez utiliser Node.js et NPM. Je ne spécifie pas explicitement une version minimale de Node.js/NPM pour l'application mais je recommande d'utiliser la dernière version LTS à partir du moment où vous configurez les choses. La version minimale de Node.js sur laquelle j'ai testé cette application est **10.16.3**.

Les installateurs peuvent être trouvés ici : [https://nodejs.org/en/download](https://nodejs.org/en/download/)

Une autre option pour installer Node est le **Gestionnaire de Versions de Node** (**nvm**), qui est un script bash conforme à POSIX pour gérer plusieurs versions actives de Node.js. Les instructions pour installer et utiliser nvm pour installer Node et NPM peuvent être trouvées à l'adresse [https://github.com/nvm-sh/nvm](https://github.com/nvm-sh/nvm).

## Installation

Le code de l'application de chat est disponible dans le dépôt [GitHub](https://github.com/) public [https://github.com/owanhunte/nodejs-chat-app](https://github.com/owanhunte/nodejs-chat-app). Clonez le dépôt dans un dossier local sur votre machine ou téléchargez et extrayez l'archive si vous n'avez pas [Git](https://git-scm.com/) installé.

Ouvrez une session de terminal, ou l'équivalent sur votre machine, et saisissez la commande suivante pour installer tous les modules Node nécessaires pour exécuter l'application :

```sh
npm install
```

## Exécuter l'application en mode développement

Après avoir effectué un `npm install`, saisissez la commande `npm run` suivante :

```sh
npm run dev
```

Cela démarrera l'application et la configurera pour écouter les connexions entrantes sur le port 3000. Ouvrez votre navigateur préféré et accédez à l'URL [http://localhost:3000/](http://localhost:3000/) pour commencer à utiliser l'application elle-même. La commande `npm run dev` exécute automatiquement l'application en utilisant le script `nodemon` donc tout changement que vous apportez au code JavaScript, CSS ou HTML de l'application redémarrera automatiquement celle-ci.

## Personnalisation du port d'écoute

Pour configurer le port sur lequel l'application écoute au démarrage, copiez le fichier `.env.example`, situé à la racine du projet, vers `.env` et définissez une valeur appropriée pour la variable d'environnement `PORT` répertoriée dans le fichier. Cela doit être fait avant que l'application ne soit démarrée.