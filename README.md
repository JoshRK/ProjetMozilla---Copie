# Site Web de Bibliothèque Locale

Ce projet est un site web simple de bibliothèque locale construit avec Express et Node.js. Il suit le [tutoriel d'introduction Express/Node de MDN](https://developer.mozilla.org/fr/docs/Learn/Server-side/Express_Nodejs/Tutorial_local_library_website).

## Table des matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Arborescence](#arborescence)
- [Tentative image](#TentativeImage)

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

