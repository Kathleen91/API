# M2L - API

### API de mise en relation du site web de la gestion des bordereaux à la base de données et à l'application mobile de réservation de salles de la Maison des Ligues de Lorraine.

Téléchargez le projet en .zip depuis le Repository AP3 et le décompresser.

Si vous ne l'avez pas déjà, téléchargez et installez NodeJS et MYSQL Workbench.

Ouvrez MYSQL Workbench, cliquez sur le bouton "Open a SQL script file in a new query tab" et sélectionnez le fichier "bdd_m2l.sql" dans le dossier ..\API\config.
En haut du script qui s'affiche, tapez les commandes "CREATE DATABASE ppe3;" et "USE ppe3;". Cliquez sur l'éclair pour créer la base de données du projet.

Ouvrez ensuite votre dossier avec Visual Studio Code.
Dans le dossier config, ouvrez le fichier db.js et remplacez "mdp" par votre mot de passe d'accès à MySQL Workbench.

Dans le terminal, entrez la commande "npm install".

A la fin du chargement, entrez la commande "npm run start". Vous obtiendrez une erreur.
Retournez dans Workbech, dans la base de données ouvrez un nouveau script et entrez les commandes "use name_database;", "ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'mdp';" et "flush privileges;".

Relancez l'API depuis le terminal de Visual Studio Code avec la commande "npm run start".

Vous pouvez directement ouvrir le site en suivant les instructions du README sur :
https://github.com/Kathleen91/API
