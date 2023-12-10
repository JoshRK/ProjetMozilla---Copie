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


## TentativeImage

Bien que j'aie initialement mis en œuvre un système d'ajout d'image via une URL, il est important de souligner que cette approche peut poser des risques de sécurité substantiels. Après avoir évalué les implications, j'ai décidé de désactiver cette fonctionnalité pour éviter tout impact négatif sur la sécurité du système.

Cependant, afin de conserver une trace de cette tentative, j'ai laissé en place le code correspondant, mais exclusivement pour le livre "Des Fleurs pour Algernon". Dans ce cas spécifique, la fonctionnalité est maintenue en raison de son succès, permettant l'affichage de la couverture du livre. Pour distinguer ce cas particulier, j'ai introduit l'attribut "cover" spécifiquement pour ce livre.

Il est crucial de noter que cette décision a été prise en toute connaissance de cause, en tenant compte des risques potentiels. Si d'autres approches plus sécurisées pour cette fonctionnalité sont envisagées à l'avenir, elles devront être mises en œuvre pour garantir la sécurité globale du système.

