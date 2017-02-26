# Contribuer à Dilia

Afin de contribuer à Dilia, il vous faudra apprendre [TypeScript](http://typescriptlang.org).
**TypeScript** est un super set de **JavaScript**. Savoir ce dernier vous aidera également.
Enfin, notre plateforme est le web: donc savoir ce qu'est le CSS et HTML vous sera aussi utile.

Pfou! Ca fait beaucoup!

Et c'est pas terminé...

Dilia utilise aussi les technologies suivantes qui vous serons utiles de connaître
un minimum:

 - Webpack
 - Angular
 - Node.js
 - Express.js

## Un client et un serveur

Dans le dossier `dilia` que vous venez de cloner, vous trouverez
l'arborescense de dossier suivante:

```bash
dilia
├── package.json            <-- Contient la liste des dépendances du projet
├── editor
│   ├── components
│   ├── modules
│   │   ├── map             <-- Code lié au cartes
│   │   ├── runner          <-- Le client Sarosa TypeScript
│   │   ...
│   └── ...
│
├── server                  <-- Le serveur web, interface de Dilia
│   ├── apis                <-- Liste des APIS exposé par le serveur
│   └── dbs/schemas         <-- Gestion de la base de données
│   └── ...
└── ...
```

Le contenu qui est servi à un browser est entièrement contenu dans le
dossier `editor`. Si vous souhaitez apporter une contribution visuelle,
ou ajouter une fonctionalité dans l'interface c'est très certainement là
qu'il faudra regarder en premier.

Tout ce qui est du type "sauvegarde de map", "synchronisation des modifications"
va vivre côté serveur et donc dans le dossier `server`.