### Correction Exercice 1 : Conversion en JSON

À partir de la table fournie, créez un tableau JSON où chaque passager est représenté par un objet avec des clés correspondant aux en-têtes de colonnes.

```json
[
  {
    "nom": "Einstein",
    "prénom": "Albert",
    "n° vol": 45622,
    "Nbr bagages": 2,
    "N° client": 154565
  },
  {
    "nom": "Lavoisier",
    "prénom": "Antoine",
    "n° vol": 45644,
    "Nbr bagages": 4,
    "N° client": 235002
  },
  {
    "nom": "Raimbault",
    "prénom": "Arthur",
    "n° vol": 12896,
    "Nbr bagages": 2,
    "N° client": 544552
  },
  {
    "nom": "Poincaré",
    "prénom": "Henri",
    "n° vol": 45644,
    "Nbr bagages": 3,
    "N° client": 781201
  },
  {
    "nom": "Lavoisier",
    "prénom": "Antoine",
    "n° vol": 45644,
    "Nbr bagages": 1,
    "N° client": 785154
  },
  {
    "nom": "Einstein",
    "prénom": "Albert",
    "n° vol": 75906,
    "Nbr bagages": 0,
    "N° client": 858547
  }
]
```

### Correction Exercice 2 : Visualisation du JSON

Après avoir sauvegardé votre fichier JSON, allez sur [JSON Viewer](http://jsonviewer.stack.hu/), chargez votre fichier `partie1.json` et visualisez la structure.

### Correction Exercice 3 : Ajout de Colonnes d'Adresse

Ajoutez une colonne `adresse` pour chaque passager. Voici comment le fichier JSON serait mis à jour :

```json
[
  // ... autres passagers
  {
    "nom": "Einstein",
    "prénom": "Albert",
    "n° vol": 75906,
    "Nbr bagages": 0,
    "N° client": 858547,
    "adresse": {
      "Num_CIV": "42",
      "Rue": "Rue du Commerce",
      "CP": "75015"
    }
  }
  // ... autres passagers
]
```

### Correction Exercice 4 : Gestion des Adresses Multiples

Pour un passager donné, ajoutez plusieurs adresses en faisant de la clé `adresse` un tableau d'objets. Pour Einstein Albert, par exemple, cela pourrait ressembler à :

```json
[
  // ... autres passagers
  {
    "nom": "Einstein",
    "prénom": "Albert",
    "n° vol": 45622,
    "Nbr bagages": 2,
    "N° client": 154565,
    "adresses": [
      {
        "Num_CIV": "123",
        "Rue": "Avenue des Champs-Élysées",
        "CP": "75008"
      },
      {
        "Num_CIV": "42",
        "Rue": "Rue de Rivoli",
        "CP": "75001"
      },
      {
        "Num_CIV": "75",
        "Rue": "Rue du Faubourg Saint-Antoine",
        "CP": "75011"
      }
    ]
  }
  // ... autres passagers
]
```


### Correction finale 

```json
[
    {
        "nom": "Einstein",
        "prénom": "Albert",
        "n° vol": 45622,
        "Nbr bagages": 2,
        "N° client": 154565,
        "adresses": [
            {
                "Num_CIV": "123",
                "Rue": "Avenue des Champs-Élysées",
                "CP": "75008"
            },
            {
                "Num_CIV": "42",
                "Rue": "Rue de Rivoli",
                "CP": "75001"
            },
            {
                "Num_CIV": "75",
                "Rue": "Rue du Faubourg Saint-Antoine",
                "CP": "75011"
            }
        ]
    },
    {
        "nom": "Lavoisier",
        "prénom": "Antoine",
        "n° vol": 45644,
        "Nbr bagages": 4,
        "N° client": 235002,
        "adresses": [
            {
                "Num_CIV": "123",
                "Rue": "Avenue des Champs-Élysées",
                "CP": "75008"
            }
        ]
    },
    {
        "nom": "Raimbault",
        "prénom": "Arthur",
        "n° vol": 12896,
        "Nbr bagages": 2,
        "N° client": 544552,
        "adresses": [
            {
                "Num_CIV": "123",
                "Rue": "Avenue des Champs-Élysées",
                "CP": "75008"
            }
        ]
    },
    {
        "nom": "Poincaré",
        "prénom": "Henri",
        "n° vol": 45644,
        "Nbr bagages": 3,
        "N° client": 781201,
        "adresses": [
            {
                "Num_CIV": "123",
                "Rue": "Avenue des Champs-Élysées",
                "CP": "75008"
            }
        ]
    },
    {
        "nom": "Lavoisier",
        "prénom": "Antoine",
        "n° vol": 45644,
        "Nbr bagages": 1,
        "N° client": 785154,
        "adresses": [
            {
                "Num_CIV": "123",
                "Rue": "Avenue des Champs-Élysées",
                "CP": "75008"
            }
        ]
    },
    {
        "nom": "Einstein",
        "prénom": "Albert",
        "n° vol": 75906,
        "Nbr bagages": 0,
        "N° client": 858547,
        "adresses": [
            {
                "Num_CIV": "123",
                "Rue": "Avenue des Champs-Élysées",
                "CP": "75008"
            }
        ]
    }
]
```