# Site Web de Bibliothèque Locale

Ce projet est un site web simple de bibliothèque locale construit avec Express et Node.js. Il suit le [tutoriel d'introduction Express/Node de MDN](https://developer.mozilla.org/fr/docs/Learn/Server-side/Express_Nodejs/Tutorial_local_library_website).

## Table des matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Arborescence](#arborescence)
- [Tentative image](#TentativeImage)
- [UML](#UML)

## Introduction

Ce projet est une mise en pratique des concepts abordés dans le [tutoriel d'introduction Express/Node de MDN](https://developer.mozilla.org/fr/docs/Learn/Server-side/Express_Nodejs/Tutorial_local_library_website). Il montre comment construire un site web de bibliothèque locale avec des fonctionnalités telles que l'affichage de la liste des livres, l'affichage des détails des livres et la gestion des instances de livres.

## Fonctionnalités

- Affichage d'une liste de livres avec leurs images de couverture
- Consultation des détails de livres individuels
- Gestion des instances de livres (par exemple, emprunter, retourner)

## Installation

1. Clonez le dépôt :

   ```bash
   git clone [adresse du repository]


2. Installez les dépendances : 

   ```bash
   npm install

3. Clonez le dépôt :

   ```bash
   npm start



Visitez http://localhost:3000/ dans votre navigateur.

Dépendances

    Express
    Mongoose
    Pug

Pour une liste complète des dépendances, consultez le fichier package.json.

## Arborescence

```vbnet
├── bin
│   ├── www.js
├── controllers
│   ├── authorController.js
│   ├── bookController.js
├── models
│   ├── author.js
│   ├── book.js
├── public
│   ├── images
│   ├── javascripts
│   ├── stylesheets
│   │   ├── style.css
├── routes
│   ├── catalog.js
│   ├── index.js
│   ├── users.js
├── views
│   ├── author_delete.pug
│   ├── author_details.pug
│   ├── author_form.pug
│   ├── author_list.pug
│   ├── book_delete.pug
│   ├── book_details.pug
│   ├── book_form.pug
│   ├── book_list.pug
│   ├── error.pug
│   ├── index.pug
│   ├── layout.pug
├── app.js
├── populatedb.js
├── wiki.js
└── .gitignore
```

## TentativeImage

Comme nous en avions discuter en cours j'ai fais plusieurs tentative pour mettre en place des images sur le site. Il est impossible de stocker des images directement sur MangoDB (du moins ce ne serait pas une bonne pratique et je n'ai pas vu de tuto qui fonctionnaient pour moi). J'ai donc tenter de mettre en place une firebase de google afin de stocker une image uploadé via le formulaire et récuperer uniquement son token comme attribut "cover" sous forme donc d'une chaine de caractère dans le schema du livre. Cependant le lien avec MangoDB était un calvaire pour essayer de faire le lien entre quel image correspondait à chaque livre j'ai donc abandonné cette solution pensant qu'elle était pas viable mais en écrivant ceci je me rend compte qu'en uploadant peut etre l'ISBN du livre associé à la cover j'aurais pu faire en sorte que cela fonctionne. 

Je me suis donc orienté sur une seconde proposition qui visait simplementt à autoriser l'utilisateur à mettre un lien d'une image dans le formulaire.

Il est important de souligner que cette approche peut poser des risques de sécurité substantiels.
Surtout du au fait que j'ai désactivé toute les vérifications du au fait que je n'arrivais pas a trouver un ensemble de vérification qui me permettrait d'assurer la sécurité.

Cependant, afin de conserver une trace de cette tentative, j'ai laissé en place le code correspondant, mais exclusivement pour le livre "Des Fleurs pour Algernon".
Il est crucial de noter que cette décision a été prise en toute connaissance de cause, en tenant compte des risques potentiels. Si d'autres approches plus sécurisées pour cette fonctionnalité sont envisagées à l'avenir, elles devront être mises en œuvre pour garantir la sécurité globale du système.

Il est donc évident qu'il ne s'agit pas la de la bonne solution.

Ce read.me sera mis à jour durant les vacances de Noël pour trouver une solution viable et permettre un affiche similaire au projet Ghibli.

## UML
