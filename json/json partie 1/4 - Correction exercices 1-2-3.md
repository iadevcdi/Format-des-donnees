### Correction de l'Exercice #1 : Transformation d'une table simple en JSON

Pour convertir la table des étudiants en format JSON, vous créez un tableau d'objets, chaque objet représentant un étudiant avec ses propriétés correspondant aux colonnes de la table.

```json
[
  {
    "ID": 1,
    "Nom": "Dupont",
    "Prénom": "Jean",
    "Âge": 23,
    "Spécialité": "Informatique"
  },
  {
    "ID": 2,
    "Nom": "Martin",
    "Prénom": "Alice",
    "Âge": 22,
    "Spécialité": "Mathématiques"
  },
  {
    "ID": 3,
    "Nom": "Leroy",
    "Prénom": "Benjamin",
    "Âge": 24,
    "Spécialité": "Physique"
  }
]
```

### Correction de l'Exercice #2 : Avec adresses composées

Lorsque vous incluez l'adresse comme un objet imbriqué, chaque objet étudiant inclura un objet `Adresse` contenant les clés pour la `Rue`, la `Ville`, et le `Code Postal` (le code postal peut être dérivé si vous le souhaitez, mais ici, il n'est pas explicitement fourni dans la table).

```json
[
  {
    "ID": 1,
    "Nom": "Dupont",
    "Prénom": "Jean",
    "Âge": 23,
    "Spécialité": "Informatique",
    "Adresse": {
      "Rue": "123, rue de la Paix",
      "Ville": "Paris"
    }
  },
  {
    "ID": 2,
    "Nom": "Martin",
    "Prénom": "Alice",
    "Âge": 22,
    "Spécialité": "Mathématiques",
    "Adresse": {
      "Rue": "456, avenue des Fleurs",
      "Ville": "Lyon"
    }
  },
  {
    "ID": 3,
    "Nom": "Leroy",
    "Prénom": "Benjamin",
    "Âge": 24,
    "Spécialité": "Physique",
    "Adresse": {
      "Rue": "789, boulevard Liberté",
      "Ville": "Marseille"
    }
  }
]
```

### Correction de l'Exercice #3 : Avec Adresses Multiples

Dans cet exercice, chaque étudiant peut avoir plusieurs adresses. Ainsi, au lieu d'un seul objet adresse, vous aurez un tableau `Adresses` pour chaque étudiant, contenant plusieurs objets adresse.

```json
[
  {
    "ID": 1,
    "Nom": "Dupont",
    "Prénom": "Jean",
    "Âge": 23,
    "Spécialité": "Informatique",
    "Adresses": [
      {
        "Type": "Domicile",
        "Rue": "123, rue de la Paix",
        "Ville": "Paris",
        "Code Postal": "75001"
      },
      {
        "Type": "Vacances",
        "Rue": "45, avenue du Lac",
        "Ville": "Annecy",
        "Code Postal": "74000"
      }
    ]
  },
  {
    "ID": 2,
    "Nom": "Martin",
    "Prénom": "Alice",
    "Âge": 22,
    "Spécialité": "Mathématiques",
    "Adresses": [
      {
        "Type": "Domicile",
        "Rue": "67, boulevard Liberté",
        "Ville": "Marseille",
        "Code Postal": "13001"
      }
    ]
  },
  {
    "ID": 3,
    "Nom": "Leroy",
    "Prénom": "Benjamin",
    "Âge": 24,
    "Spécialité": "Physique",
    "Adresses": [
      {
        "Type": "Domicile",
        "Rue": "89, chemin des Bois",
        "Ville": "Bordeaux",
        "Code Postal": "33000"
      },
      {
        "Type": "Secondaire",
        "Rue": "2, impasse du Château",
        "Ville": "Saint-Émilion",
        "Code Postal": "33330"
      }
    ]
  }
]
```
