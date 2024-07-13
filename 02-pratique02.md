## Examen : Analyse comparative des méthodes de clustering pour la détection de chutes

### Objectif :
Comparer l'efficacité de K-means, DBSCAN et le clustering hiérarchique pour la détection non supervisée de chutes en utilisant plusieurs datasets différents.

### Datasets :
1. **Le2i Fall Dataset** : [Lien vers le dataset](https://www.kaggle.com/datasets/tuyenldvn/falldataset-imvia)
   - Ce dataset contient des vidéos de chutes et d'activités quotidiennes.
   - Il offre une variété de scénarios de chutes et d'activités normales.
   - Vous pouvez extraire des caractéristiques de mouvement à partir des vidéos.
   - Il permet de tester la capacité de l'algorithme à distinguer les chutes des activités normales sans utiliser les étiquettes.

2. **Fall Detection Dataset** : [Lien vers le dataset](https://www.kaggle.com/datasets/uttejkumarkandagatla/fall-detection-dataset)
   - Ce dataset contient des images de chutes et d'activités normales.
   - Vous pouvez extraire des caractéristiques visuelles des images.
   - Il permet de tester si l'algorithme peut regrouper naturellement les images de chutes et d'activités normales.
   - La nature statique des images peut offrir un défi différent par rapport aux données de mouvement.

3. **CAUCAFall Dataset** :
   - Ce dataset simule des chutes dans un environnement non contrôlé, ce qui est plus proche des conditions réelles.
   - Il pourrait offrir une plus grande variabilité dans les données, testant ainsi la capacité de l'algorithme à gérer des scénarios complexes.

4. **Walker Fall Detection Dataset** :
   - Ce dataset contient des données inertielles de personnes utilisant des déambulateurs.
   - Il fournit des données de mouvement sans étiquettes prédéfinies.
   - Idéal pour appliquer DBSCAN ou K-means.

5. **KFall Dataset** :
   - Offre 11 colonnes incluant des données d'accéléromètre, de gyroscope et d'angles d'Euler.
   - Bien qu'il contienne des étiquettes, vous pouvez ignorer ces informations pour une approche non supervisée.

6. **Inertial Measurement Unit Fall Detection Dataset (IMU Dataset)** :
   - Fournit des données d'accélération, de vitesse angulaire et de champs magnétiques à 128 Hz provenant de 7 emplacements corporels.
   - Ce jeu de données riche est parfait pour tester différentes méthodes de clustering.

7. **Dataset de l'ARCO Research Group** :
   - Comprend des fichiers CSV avec des accélérations, des rotations et des orientations absolues collectées à partir d'un capteur monté à la taille.
   - Peut être utilisé en ignorant les étiquettes d'activité pour une approche non supervisée.

### Tâches :
#### 1. Prétraitement des données :
   - Pour chaque dataset, extraire des caractéristiques pertinentes (mouvements pour les vidéos, descripteurs visuels pour les images).
   - Normaliser les données si nécessaire.

#### 2. Application des algorithmes de clustering :
   - Appliquer K-means, DBSCAN et le clustering hiérarchique sur chaque dataset.
   - Pour K-means et le clustering hiérarchique, tester différents nombres de clusters (par exemple, de 2 à 10).
   - Pour DBSCAN, expérimenter avec différentes valeurs d'epsilon et de min_samples.

#### 3. Évaluation de la qualité du clustering :
   - Pour K-means : Utiliser l'Analyse en Composantes Principales (PCA) pour visualiser les clusters en 2D ou 3D.
   - Pour tous les algorithmes : Calculer et comparer les scores de silhouette.
   - Calculer l'indice de Dunn et l'indice de Davies-Bouldin pour chaque résultat de clustering.

#### 4. Analyse comparative :
   - Comparer les performances des trois algorithmes sur chaque dataset en utilisant les métriques calculées.
   - Analyser comment les performances varient entre les différents datasets.
   - Discuter des avantages et des inconvénients de chaque méthode pour la détection de chutes.

#### 5. Interprétation des résultats :
   - Pour chaque dataset et méthode, interpréter les clusters obtenus. Peuvent-ils être associés à des chutes ou à des activités normales ?
   - Discuter de la pertinence de l'approche non supervisée pour la détection de chutes.

#### 6. Rapport et présentation :
   - Rédiger un rapport détaillant la méthodologie, les résultats et les conclusions.
   - Préparer une présentation visuelle des résultats les plus significatifs.

### Bonus :
   - Explorer d'autres méthodes de réduction de dimensionnalité (t-SNE, UMAP) pour la visualisation des clusters.
   - Proposer et implémenter une méthode pour déterminer automatiquement le nombre optimal de clusters pour K-means et le clustering hiérarchique.

### Citations :
1. [Machine Learning Clustering DBSCAN](https://datascientest.com/machine-learning-clustering-dbscan)

2. [Kaggle - Machine Learning Non Supervisé](https://www.kaggle.com/code/zoupet/machine-learning-non-supervis-correction)

3. [Principaux Algorithmes d'Apprentissage Non Supervisé](https://fr.linedata.com/principaux-algorithmes-dapprentissage-non-supervise)

4. [Apprentissage Non Supervisé de Flux de Données Massives](https://www.researchgate.net/publication/333772967_Apprentissage_non_supervise_de_flux_de_donnees_massives_application_aux_Big_Data_d%27assurance)

5. [Discovery Unsupervised Learning](https://fr.mathworks.com/discovery/unsupervised-learning.html)
