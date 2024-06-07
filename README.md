face recognition app

Cette application detecte les visages en se basant sur un API de Clarifai. 

Pour la faire fonctionner, j'ai cree deux tableaux login et users dans model de donnees postgres, communicant par REST API via knex.js, et en utilisant des packages de hash bcrypt-nodejs et en le securisant par un autre package CORS, les appels http sont geres par la librairie express JS.

Pour la communication avec le Front End, j'ai utilise le package body-parser pour convertir de json a string, mais la derniere version d'express JS vient avec body parser.