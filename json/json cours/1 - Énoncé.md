# Gestion des Données Passagers pour un Aéroport

## Introduction

Ce projet a pour but de vous familiariser avec le format JSON. Vous transformerez des données tabulaires représentant les informations des passagers d'un aéroport en un format exploitable pour des applications web ou mobiles.

## Exercices

### Exercice 1 : Conversion en JSON

**Objectif** : Convertir une table de données passagers en format JSON.

**Table de données** :

| nom       | prénom    | n° vol | Nbr bagages | N° client |
|-----------|-----------|--------|-------------|-----------|
| Einstein  | Albert    | 45622  | 2           | 154565    |
| Lavoisier | Antoine   | 45644  | 4           | 235002    |
| Raimbault | Arthur    | 12896  | 2           | 544552    |
| Poincaré  | Henri     | 45644  | 3           | 781201    |
| Lavoisier | Antoine   | 45644  | 1           | 785154    |
| Einstein  | Albert    | 75906  | 0           | 858547    |

**Instructions** :
- Transformez la table ci-dessus en une structure JSON.

**Résultat attendu** : Un fichier JSON nommé `partie1.json`.

### Exercice 2 : Visualisation du JSON

**Objectif** : Visualiser le fichier JSON créé à l'aide d'un outil en ligne.

**Instructions** :
- Utilisez l'outil [JSON Viewer](http://jsonviewer.stack.hu/) pour visualiser le fichier `partie1.json`.

### Exercice 3 : Ajout de Colonnes d'Adresse

**Objectif** : Ajouter des informations d'adresse détaillées pour chaque passager dans le fichier JSON.

**Nouvelles données à inclure** :

- `Num_CIV` : Numéro civique
- `Rue` : Nom de la rue
- `CP` : Code postal

**Instructions** :
- Modifiez le fichier JSON pour inclure une colonne `adresse` contenant les nouvelles données pour chaque passager.

**Résultat attendu** : Un fichier JSON mis à jour nommé `partie1.json` avec les adresses ajoutées.

### Exercice 4 : Gestion des Adresses Multiples

**Objectif** : Ajouter plusieurs adresses pour un passager donné.

**Instructions** :
- Modifiez le fichier JSON pour permettre à au moins un passager d'avoir plusieurs adresses.
- Chaque adresse doit suivre la structure définie dans l'exercice précédent.

**Résultat attendu** : Un fichier JSON nommé `partie3.json` contenant des adresses multiples pour certains passagers.

**Visualisation** :
- Utilisez [JSON Viewer](http://jsonviewer.stack.hu/) pour visualiser le fichier `partie3.json`.
