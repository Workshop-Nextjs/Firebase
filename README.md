# Firebase

BONJOUR !! 😁
Bienvenue à ce sublime workshop où nous allons apprendre à deployer un site web Nextjs avec différents hébergeur

## Commençons avec Firebase

- Créer un compte sur firebase (lol)
- Aller dans la catégorie hosting
- Créer un nouveau projet (Étape 3 décocher les Analytics !!!)

Suivre toutes les étapes de l'étape 4
Exécuter 
```
firebase login
firebase init
```

- Connectez-vous avec la même adresse mail que vous avez utiliser pour créer le compte firebase
- Choisir : Hosting: Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys
- Use an existing project
- Choisir le projet
- 3xEnter

Après la génération du fichier firebase.json, il faudra remplacer
```
"public": "public",

"public": "./out",
```

```
yarn build
yarn export
```

Comme vous pouvez le constater il y a un soucis vous ne pouvez pas exporter

Vous allez devoir effectuer quelques modifications

- https://nextjs.org/docs/advanced-features/static-html-export
- https://firebase.google.com/products/functions?gclid=CjwKCAjwy_aUBhACEiwA2IHHQBMNl4vodf-3SmEGhUwjJnBWaE9MMURzWLnP_8oLyYD5eg6rFzfsfRoCLVgQAvD_BwE&gclsrc=aw.ds

- https://nextjs.org/docs/messages/export-image-api

Réessayer de build et d'export jusqu'à ce que ça marche
