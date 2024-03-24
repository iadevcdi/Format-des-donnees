D'accord, changeons de contexte et utilisons l'exemple d'un aéroport pour proposer un nouvel ensemble d'exercices progressifs. Ensuite, je fournirai directement la correction pour chaque étape.

---

# Exercices : Gestion de Données d'Aéroport en JSON

## Exercice #1 : Enregistrement des Vols

### Objectif
Convertir une table simple de vols en format JSON.

### Table de données

| Numéro de Vol | Compagnie Aérienne | Destination | Heure de Départ |
|---------------|--------------------|-------------|-----------------|
| AF115         | Air France         | Paris       | 10:30           |
| BA216         | British Airways    | Londres     | 12:45           |
| DL400         | Delta Airlines     | New York    | 15:00           |

### Correction

```json
[
  {
    "Numéro de Vol": "AF115",
    "Compagnie Aérienne": "Air France",
    "Destination": "Paris",
    "Heure de Départ": "10:30"
  },
  {
    "Numéro de Vol": "BA216",
    "Compagnie Aérienne": "British Airways",
    "Destination": "Londres",
    "Heure de Départ": "12:45"
  },
  {
    "Numéro de Vol": "DL400",
    "Compagnie Aérienne": "Delta Airlines",
    "Destination": "New York",
    "Heure de Départ": "15:00"
  }
]
```

## Exercice #2 : Enregistrement des Vols avec Détails Supplémentaires

### Objectif
Ajouter des détails supplémentaires sur chaque vol, tels que la porte d'embarquement et le statut du vol.

### Table de données

| Numéro de Vol | Compagnie Aérienne | Destination | Heure de Départ | Porte d'Embarquement | Statut         |
|---------------|--------------------|-------------|-----------------|----------------------|----------------|
| AF115         | Air France         | Paris       | 10:30           | 24A                  | À l'heure      |
| BA216         | British Airways    | Londres     | 12:45           | 18C                  | Retardé        |
| DL400         | Delta Airlines     | New York    | 15:00           | 30B                  | Annulé         |

### Correction

```json
[
  {
    "Numéro de Vol": "AF115",
    "Compagnie Aérienne": "Air France",
    "Destination": "Paris",
    "Heure de Départ": "10:30",
    "Porte d'Embarquement": "24A",
    "Statut": "À l'heure"
  },
  {
    "Numéro de Vol": "BA216",
    "Compagnie Aérienne": "British Airways",
    "Destination": "Londres",
    "Heure de Départ": "12:45",
    "Porte d'Embarquement": "18C",
    "Statut": "Retardé"
  },
  {
    "Numéro de Vol": "DL400",
    "Compagnie Aérienne": "Delta Airlines",
    "Destination": "New York",
    "Heure de Départ": "15:00",
    "Porte d'Embarquement": "30B",
    "Statut": "Annulé"
  }
]
```

## Exercice #3 : Enregistrement des Vols avec Passagers

### Objectif
Ajouter une liste de passagers pour chaque vol, où chaque passager a un nom et un numéro de siège.

### Tables de données

**Vols**

| Numéro de Vol | Compagnie Aérienne | Destination | Heure de Départ |
|---------------|--------------------|-------------|-----------------|
| AF115         | Air France         | Paris       | 10:30           |
| BA216         | British Airways    | Londres     | 12:45           |

**Passagers (AF115)**

| Nom         | Numéro de Siège |
|-------------|-----------------|
| Marie Dupont| 12A             |
| Jean Durand | 12B             |

**Passagers (BA216)**

| Nom           | Numéro de Siège |
|---------------|-----------------|
| Alice Martin  | 15C             |
| David Johnson | 15D             |

### Correction

```json
[
  {
    "Numéro de Vol": "AF115",
    "Compagnie Aérienne": "Air France",
    "Destination": "Paris",
    "Heure de Départ": "10:30",
    "Passagers": [
      {
        "Nom": "Marie Dupont",
        "Numéro de Siège": "12A"
      },
      {
        "Nom": "Jean Durand",
        "Numéro de Siège": "12B"
      }
    ]
  },
  {
    "Numéro de Vol": "BA216",
    "Compagnie Aérienne": "British Airways",
    "Destination": "Londres",
    "Heure de Départ": "12:45",
    "Passagers": [
      {
        "Nom": "Alice Martin",
        "Numéro de Siège": "15C"
      },
      {
        "Nom": "David Johnson",
        "Numéro de Siège": "15D"
      }
    ]
  }
]
```
