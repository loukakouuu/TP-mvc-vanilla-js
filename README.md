# Architecture MVC en JavaScript natif

> Projet scolaire. Une liste de tâches implémentée sans aucun framework, pour
> mettre en pratique le patron **MVC** et deux patrons de conception classiques.

## Le principe

L'application est découpée en trois fichiers qui ne se connaissent que par leurs
interfaces :

| Fichier | Rôle |
|---|---|
| [`model.js`](model.js) | Les données et la logique métier. Ne sait rien de l'affichage. |
| [`view.js`](view.js) | Le rendu et les écouteurs d'événements. Ne sait rien des données. |
| [`controller.js`](controller.js) | Le pont entre les deux. |

## Patrons mis en œuvre

- **MVC** — séparation stricte des responsabilités
- **Singleton** — `TaskModel` garantit une instance unique de la source de données
- **Héritage** — `AdvancedTask` étend `BaseTask` en ajoutant la catégorie

## Fonctionnalités

Ajout de tâches, catégorisation (travail / maison / divers), suppression.

## Lancer le projet

Aucune dépendance, aucun build : ouvrir [`index.html`](index.html) dans un
navigateur.

## Licence

[MIT](LICENSE)
