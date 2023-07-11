# Readme - Projet Angular Nest avec TypeORM et PostgreSQL

Ce projet est un simple "Todo App" avec des fonctionnalités de CRUD (Create, Read, Update, Delete) et d'authentification. Il utilise les technologies suivantes :

- Angular : un framework de développement d'applications web côté client
- NestJS : un framework de développement d'applications web côté serveur basé sur Node.js
- TypeORM : un ORM (Object Relational Mapping) pour les bases de données relationnelles en TypeScript
- PostgreSQL : un système de gestion de base de données relationnelle

## Prérequis

Avant de commencer, assurez-vous d'avoir les éléments suivants installés sur votre machine :

- Node.js : [Installer Node.js](https://nodejs.org/)
- Angular CLI : [Installer Angular CLI](https://angular.io/cli)
- PostgreSQL : [Installer PostgreSQL](https://www.postgresql.org/download/)

## Installation

1. Cloner le projet depuis le repository Git :

   ```
   git clone <repository_url>
   ```

2. Installer les dépendances du projet :

   ```
   cd <project_folder>
   npm install
   ```

## Configuration de la base de données

1. Créer une base de données PostgreSQL vide pour le projet.

2. Configurer la connexion à la base de données dans le fichier `ormconfig.json`. Remplacez les valeurs suivantes par les informations de votre base de données :

   ```
   {
     "type": "postgres",
     "host": "localhost",
     "port": 5432,
     "username": "<your_username>",
     "password": "<your_password>",
     "database": "<your_database>",
     "entities": ["dist/**/*.entity{.ts,.js}"],
     "synchronize": true
   }
   ```

## Lancement du projet

1. Compiler le projet Angular :

   ```
   ng build
   ```

2. Lancer le serveur NestJS :

   ```
   npm start
   ```

3. Accéder à l'application dans votre navigateur à l'adresse `http://localhost:3000`.

## Documentation complémentaire

Pour en savoir plus sur les différentes technologies utilisées dans ce projet, consultez les liens suivants :

- Angular : [Documentation officielle](https://angular.io/docs)
- NestJS : [Documentation officielle](https://docs.nestjs.com/)
- TypeORM : [Documentation officielle](https://typeorm.io/#/)
- PostgreSQL : [Documentation officielle](https://www.postgresql.org/docs/)

## Autres ressources

- [NestJS Tutorial: Build your First REST API CRUD App with TypeORM](https://www.techiediaries.com/nestjs-tutorial-rest-api-crud/)
- [TypeORM database migrations in NestJS apps](https://anjith-p.medium.com/typeorm-database-migrations-in-nestjs-apps-ace923edf1bf)

N'hésitez pas à consulter ces ressources pour obtenir plus d'informations sur la création d'une application CRUD avec NestJS, TypeORM et PostgreSQL.