# Exercice #3 Avancé : Transformation d'une table en JSON avec Adresses Multiples

## Objectif

Cet exercice avancé vise à renforcer votre compréhension du format JSON en gérant des structures de données plus complexes. Vous convertirez une table d'étudiants, où chaque étudiant peut avoir plusieurs adresses, en une structure JSON.

## Table de Données

Vous avez à disposition la table suivante qui répertorie des informations sur des étudiants, et cette fois, chaque étudiant peut avoir plusieurs adresses.

### Étudiants

| ID | Nom      | Prénom   | Âge | Spécialité       |
|----|----------|----------|-----|------------------|
| 1  | Dupont   | Jean     | 23  | Informatique     |
| 2  | Martin   | Alice    | 22  | Mathématiques    |
| 3  | Leroy    | Benjamin | 24  | Physique         |

### Adresses

| ID Étudiant | Type       | Rue                   | Ville         | Code Postal |
|-------------|------------|-----------------------|---------------|-------------|
| 1           | Domicile   | 123, rue de la Paix   | Paris         | 75001       |
| 1           | Vacances   | 45, avenue du Lac     | Annecy        | 74000       |
| 2           | Domicile   | 67, boulevard Liberté | Marseille     | 13001       |
| 3           | Domicile   | 89, chemin des Bois   | Bordeaux      | 33000       |
| 3           | Secondaire | 2, impasse du Château | Saint-Émilion | 33330       |

## Instructions

Votre tâche est de transformer ces tables en une structure de données JSON, en respectant les relations entre étudiants et adresses.

1. **Créez un tableau JSON pour les étudiants** : Ce tableau contiendra chaque étudiant.

2. **Intégrez les adresses comme un tableau d'objets** : Pour chaque étudiant, ajoutez un champ "Adresses" qui est un tableau contenant toutes ses adresses.

3. **Structurez chaque adresse comme un objet JSON** : Chaque adresse sera représentée par un objet JSON avec des clés correspondant aux colonnes de la table Adresses (Type, Rue, Ville, Code Postal).
