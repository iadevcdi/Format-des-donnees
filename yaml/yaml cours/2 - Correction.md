### Correction Exercice 1 : Conversion de Données Tabulaires en YAML

```yaml
passagers:
  - nom: Einstein
    prénom: Albert
    n°_vol: 45622
    nbr_bagages: 2
    n°_client: 154565
  - nom: Lavoisier
    prénom: Antoine
    n°_vol: 45644
    nbr_bagages: 4
    n°_client: 235002
  - nom: Raimbault
    prénom: Arthur
    n°_vol: 12896
    nbr_bagages: 2
    n°_client: 544552
  - nom: Poincaré
    prénom: Henri
    n°_vol: 45644
    nbr_bagages: 3
    n°_client: 781201
  - nom: Lavoisier
    prénom: Antoine
    n°_vol: 45644
    nbr_bagages: 1
    n°_client: 785154
  - nom: Einstein
    prénom: Albert
    n°_vol: 75906
    nbr_bagages: 0
    n°_client: 858547
```

### Correction Exercice 2 : Ajout d'Informations d'Adresse

```yaml
passagers:
  - nom: Einstein
    prénom: Albert
    n°_vol: 45622
    nbr_bagages: 2
    n°_client: 154565
    adresse:
      Num_CIV: "10"
      Rue: "Rue de l'Univers"
      CP: "75005"
  # Ajouter les adresses pour les autres passagers en suivant le même modèle
```
# Correction complète
```yaml
passagers:
  - nom: Einstein
    prénom: Albert
    n°_vol: 45622
    nbr_bagages: 2
    n°_client: 154565
    adresses:
      - Num_CIV: "10"
        Rue: "Rue de l'Univers"
        CP: "75005"
      - Num_CIV: "42"
        Rue: "Rue Newton"
        CP: "75008"
  - nom: Lavoisier
    prénom: Antoine
    n°_vol: 45644
    nbr_bagages: 4
    n°_client: 235002
    adresses:
      - Num_CIV: "25"
        Rue: "Avenue des Chimistes"
        CP: "75007"
  - nom: Raimbault
    prénom: Arthur
    n°_vol: 12896
    nbr_bagages: 2
    n°_client: 544552
    adresses:
      - Num_CIV: "58"
        Rue: "Rue du Laboratoire"
        CP: "75015"
  - nom: Poincaré
    prénom: Henri
    n°_vol: 45644
    nbr_bagages: 3
    n°_client: 781201
    adresses:
      - Num_CIV: "33"
        Rue: "Boulevard de l'Infini"
        CP: "75014"
  - nom: Lavoisier
    prénom: Antoine
    n°_vol: 45644
    nbr_bagages: 1
    n°_client: 785154
    adresses:
      - Num_CIV: "25"
        Rue: "Avenue des Chimistes"
        CP: "75007"
  - nom: Einstein
    prénom: Albert
    n°_vol: 75906
    nbr_bagages: 0
    n°_client: 858547
    adresses:
      - Num_CIV: "160"
        Rue: "Rue de l'Université"
        CP: "75006"

```

### Correction Exercice 3 : Gestion des Adresses Multiples

```yaml
passagers:
  - nom: Einstein
    prénom: Albert
    n°_vol: 45622
    nbr_bagages: 2
    n°_client: 154565
    adresses:
      - Num_CIV: "10"
        Rue: "Rue de l'Univers"
        CP: "75005"
      - Num_CIV: "21"
        Rue: "Rue de la Paix"
        CP: "75002"
  # Continuer avec les informations d'adresse pour les autres passagers
  # Pour ceux qui ont plusieurs adresses, utilisez le format de liste d'adresses comme montré ci-dessus
```


# Correction complète

```yaml
passagers:
  - nom: Einstein
    prénom: Albert
    n°_vol: 45622
    nbr_bagages: 2
    n°_client: 154565
    adresses:
      - Num_CIV: "10"
        Rue: "Rue de l'Univers"
        CP: "75005"
      - Num_CIV: "21"
        Rue: "Rue de la Paix"
        CP: "75002"
  - nom: Lavoisier
    prénom: Antoine
    n°_vol: 45644
    nbr_bagages: 4
    n°_client: 235002
    adresses:
      - Num_CIV: "33"
        Rue: "Rue des Alchimistes"
        CP: "75006"
  - nom: Raimbault
    prénom: Arthur
    n°_vol: 12896
    nbr_bagages: 2
    n°_client: 544552
    adresses:
      - Num_CIV: "58"
        Rue: "Rue des Explorateurs"
        CP: "75014"
  - nom: Poincaré
    prénom: Henri
    n°_vol: 45644
    nbr_bagages: 3
    n°_client: 781201
    adresses:
      - Num_CIV: "75"
        Rue: "Boulevard des Philosophes"
        CP: "75007"
  - nom: Lavoisier
    prénom: Antoine
    n°_vol: 45644
    nbr_bagages: 1
    n°_client: 785154
    adresses:
      - Num_CIV: "12"
        Rue: "Place des Chimistes"
        CP: "75005"
  - nom: Einstein
    prénom: Albert
    n°_vol: 75906
    nbr_bagages: 0
    n°_client: 858547
    adresses:
      - Num_CIV: "160"
        Rue: "Avenue de la Science"
        CP: "75008"
```

