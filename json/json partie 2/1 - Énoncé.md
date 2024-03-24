# Exercices de Transformation de Données JSON dans le Contexte Aéroportuaire

## Introduction

Ces exercices sont conçus pour vous aider à maîtriser la transformation de données tabulaires en format JSON, en utilisant le contexte des aéroports et de leurs vols. Vous commencerez par transformer une simple table d'aéroports, puis ajouterez des informations d'adresse, et enfin gérerez des enregistrements de vols multiples pour chaque aéroport.

### Exercice #1 : Liste d'Aéroports

#### Objectif

Convertir une table d'aéroports en format JSON.

#### Table de données

| ID | Nom                     | Ville       | Pays        |
|----|-------------------------|-------------|-------------|
| 1  | Aéroport Charles de Gaulle | Paris       | France      |
| 2  | Aéroport Heathrow       | Londres     | Royaume-Uni |
| 3  | Aéroport John F. Kennedy | New York    | États-Unis  |

#### Instructions

Transformez cette table en une structure JSON où chaque aéroport est un objet dans un tableau.

### Exercice #2 : Aéroports avec Adresse

#### Objectif

Ajouter un niveau de complexité en incluant des détails d'adresse pour chaque aéroport.

#### Table de données

| ID | Nom                     | Adresse                                   | Ville       | Pays        |
|----|-------------------------|-------------------------------------------|-------------|-------------|
| 1  | Aéroport Charles de Gaulle | Roissypôle, 95700 Roissy-en-France | Paris       | France      |
| 2  | Aéroport Heathrow       | Longford TW6                              | Londres     | Royaume-Uni |
| 3  | Aéroport John F. Kennedy | Queens, NY 11430                          | New York    | États-Unis  |

#### Instructions

Pour chaque aéroport, créez un objet JSON, incluant l'adresse comme un objet imbriqué avec des clés pour l'Adresse, la Ville, et le Pays.

### Exercice #3 : Aéroports avec Vols Multiples

#### Objectif

Gérer des structures de données plus complexes en permettant à chaque aéroport d'avoir plusieurs vols disponibles.

#### Tables de données

**Aéroports**

| ID | Nom                     | Ville       | Pays        |
|----|-------------------------|-------------|-------------|
| 1  | Aéroport Charles de Gaulle | Paris       | France      |
| 2  | Aéroport Heathrow       | Londres     | Royaume-Uni |
| 3  | Aéroport John F. Kennedy | New York    | États-Unis  |

**Vols**

| ID Aéroport | Numéro de Vol | Destination         | Heure de Départ |
|-------------|---------------|---------------------|-----------------|
| 1           | AF22          | New York            | 08:30           |
| 1           | AF98          | San Francisco       | 15:45           |
| 2           | BA15          | Sydney              | 22:00           |
| 3           | AA101         | Los Angeles         | 07:00           |
| 3           | DL400         | Atlanta             | 09:30           |

#### Instructions

Pour chaque aéroport, créez un champ "Vols" qui est un tableau contenant tous ses vols disponibles. Chaque vol doit être un objet JSON avec des clés pour le Numéro de Vol, la Destination, et l'Heure de Départ.
