# Exercice #2 : Transformation d'une table en JSON avec adresses composées

## Objectif

Dans cet exercice, vous approfondirez votre compréhension du format JSON en convertissant une table de données plus complexe en un objet JSON. Cette table inclut des informations d'adresse pour chaque étudiant, ce qui ajoute un niveau d'imbriquement à la structure JSON.

## Table de données

Considérez la table suivante, qui liste des informations sur des étudiants, y compris leurs adresses :

| ID | Nom      | Prénom   | Âge | Spécialité    | Adresse                          |
|----|----------|----------|-----|---------------|----------------------------------|
| 1  | Dupont   | Jean     | 23  | Informatique  | 123, rue de la Paix, Paris       |
| 2  | Martin   | Alice    | 22  | Mathématiques | 456, avenue des Fleurs, Lyon    |
| 3  | Leroy    | Benjamin | 24  | Physique      | 789, boulevard Liberté, Marseille |

## Instructions

1. **Créez un tableau JSON** : Commencez par créer un tableau JSON pour stocker les objets représentant chaque étudiant.

2. **Transformez chaque ligne en un objet JSON**, incluant l'adresse comme un objet imbriqué. Chaque étudiant sera représenté par un objet JSON, où l'adresse est elle-même un objet avec des clés pour la rue, la ville, et le code postal.

3. **Structurez l'adresse** : Pour l'adresse, séparez la rue, la ville, et le code postal dans des champs distincts au sein d'un objet "Adresse". Utilisez votre jugement pour déterminer le format de ces champs à partir des informations fournies.
