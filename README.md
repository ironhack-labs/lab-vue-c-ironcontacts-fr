![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | Vue.js IronContacts (Composition API)

## Introduction

Après ton passage à Ironhack, tu as décidé de travailler dans l'industrie du cinéma et tu as trouvé un emploi où tu dois gérer les contacts d'un célèbre producteur.

Ta tâche consiste à créer une application de gestion des contacts pour ce producteur en utilisant Vue.js.

## Configuration

- Fork ce repo
- Clone ce repo
- Ouvre le LAB et commence :

  ```bash
  $ cd lab-vue-c-ironcontacts
  $ npm install
  $ npm run dev
  ```


## Remise

- Une fois terminé, exécute les commandes suivantes :

  ```bash
  git add .
  git commit -m "done"
  git push origin main
  ```

- Crée une Pull Request pour que tes TAs puissent vérifier ton travail.


## Getting Started (Pour commencer)

Nettoie le composant `App.js` pour qu'il ait la structure suivante :

```js
// src/App.vue
<template>
</template>

<script setup>
</script>

<style>
</style>
```

## Instructions

### Itération 1 | Afficher 5 contacts

Commençons par examiner le code de départ.

Dans le dossier `src`, nous avons un fichier `contacts.json` contenant les contacts du producteur. Importe le fichier `contacts.json` dans `App.vue`. Une fois cela fait, crée une variable de référence nommée `contacts` qui stocke un **tableau contenant les 5 premiers contacts**.

Affiche ce tableau de 5 contacts sous forme de liste dans une `<table>` et affiche l'`image`, le `nom` et la `popularité` de chaque contact.

Pour l'instant, rends le contenu dans `App.vue`. Cependant, ne crée pas encore de composant dédié pour la liste de contacts. Pour l'instant, rends simplement tout dans un seul composant.

Continuons.

Pour importer `contacts.json` dans `App.vue`, tu peux utiliser :

```js
import contacts from "./contacts.json";
```

À la fin de cette itération, ton application devrait ressembler à ceci :

<details>
  <summary> Clique ici pour voir l'image - Itération 1</summary>

![Screenshot - Iteration 1](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-1.png)

</details>

### Itération 2 | Afficher conditionnellement les informations des prix

Le producteur souhaite voir les informations sur les _récompenses_ que chaque contact a remportées.

Met à jour la liste et ajoute deux colonnes supplémentaires "A remporté un Oscar" et "A remporté un Emmy", à la fin de la table. Ensuite, en fonction de la valeur `wonOscar` et `wonEmmy` de chaque contact, affiche conditionnellement une icône de trophée :trophy: ou aucun contenu.

Une fois terminé, ton application devrait ressembler à ceci :

<details>

<summary> Clique ici pour voir l'image - Itération 2</summary>

![Screenshot - Iteration 2](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-2.png)

</details>

### Itération 3 | Ajouter de nouveaux contacts aléatoires

Dans ton application, crée un bouton "Ajouter un contact aléatoire". À chaque fois que tu cliques sur ce bouton, un nouveau contact aléatoire doit être ajouté aux `contacts`. Tu dois obtenir des contacts aléatoires à partir des contacts restants qui ne sont pas encore affichés.

Tout d'abord, sélectionne aléatoirement un contact parmi le tableau des contacts restants. Ensuite, ajoute ce contact au tableau qui se trouve dans ta variable de référence des données (c'est le tableau des 5 premiers contacts précédemment créé).

À la fin de cette itération, ton site web devrait ressembler à cela :

<details>
  <summary> Clique ici pour voir l'image - Itération 3 </summary>

![Screenshot - Iteration 3](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-3.png)

</details>

### Itération 4 | Trier les contacts par nom et popularité

Le producteur t'a demandé d'ajouter deux nouveaux boutons pour l'aider à trier ses contacts. Lorsque tu cliques sur l'un des boutons, cela doit **trier la table par `nom`** (par ordre alphabétique), et lorsque tu cliques sur l'autre, cela doit **trier par `popularité`** (du plus élevé au plus bas).

Une fois que tu as trié le tableau, n'oublie pas de mettre à jour la variable de référence qui contient les contacts.

Voici à quoi ton application devrait ressembler à la fin de cette itération :

<details>
  <summary> Clique ici pour voir l'image - Itération 4 </summary>

![Screenshot - Iteration 4](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-4.png)

</details>

### Itération 5 | Supprimer des contacts

Le producteur souhaite également supprimer certains de ses contacts. Implémente un bouton "Supprimer" sur chaque ligne de ta `<table>` qui permettra à l'utilisateur de supprimer le contact sur lequel il a cliqué.

Lorsqu'il clique, tu dois obtenir l'`id` de cet acteur et l'utiliser pour supprimer le contact du tableau. N'oublie pas de mettre à jour la variable de référence qui contient les contacts après avoir supprimé le contact !

Une fois terminé, ton application devrait ressembler à cela (après avoir joué un peu avec le bouton _Supprimer_) :

<details>
  <summary> Clique ici pour voir l'image - Itération 5 </summary>

![Screenshot - Iteration 5](https://education-team-2020.s3.eu-west-1.amazonaws.com/web-dev/labs/lab-react-ironcontacts-5.png)

</details>

### Itération 6 | Bonus | Mise en forme

Malheureusement, cette liste de contacts n'est pas prête pour la production. Nous sommes dans l'industrie du cinéma ! Elle doit briller ! Ajoute un peu de CSS pour rendre l'application attrayante.

<br>

Bon codage ! :blue_heart: