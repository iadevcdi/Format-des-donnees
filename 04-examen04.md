# Examen : Analyse comparative des méthodes de clustering pour la détection de chutes

### Objectif :
Comparer l'efficacité de K-means, DBSCAN et le clustering hiérarchique pour la détection non supervisée des activités journalères comme s'assoir, walking, sitting, chutes en utilisant un ou deux datasets parmi ceux proposés.

### Datasets :
1. **Le2i Fall Dataset** : [Lien vers le dataset](https://www.kaggle.com/datasets/tuyenldvn/falldataset-imvia)
2. **Fall Detection Dataset** : [Lien vers le dataset](https://www.kaggle.com/datasets/uttejkumarkandagatla/fall-detection-dataset)
3. **CAUCAFall Dataset**
4. **Walker Fall Detection Dataset**
5. **KFall Dataset**
6. **Inertial Measurement Unit Fall Detection Dataset (IMU Dataset)**
7. **Dataset de l'ARCO Research Group**

### Annexes :
- **Pour K-means :**
  - Utilisez la méthode du coude pour déterminer le nombre optimal de clusters.
  - Visualisez les clusters.
  - Appliquez l'Analyse en Composantes Principales (PCA) pour visualiser les clusters en 2D ou 3D pour valider les résultats.
  - Pour la tâche 3, vous n'êtes pas obligés d'appliquer nécessairement le score de silhouette. Si vous trouvez un score plus intéressant ou complémentaire (comme le Dunn ou l'indice de Davies-Bouldin), vous pouvez l'appliquer en justifiant votre choix.

### Tâches :
1. **Prétraitement des données :**
   - Choisissez un dataset parmi ceux proposés.
   - Extrayez des caractéristiques pertinentes et normalisez les données si nécessaire.

2. **Application des algorithmes de clustering :**
   - Appliquez chacun des 3 algorithmes (K-means, DBSCAN et le clustering hiérarchique) sur le dataset choisi.

3. **Évaluation de la qualité du clustering :**
   - Calculez et comparez les scores de silhouette pour chaque algorithme appliqué.
   - Si vous trouvez d'autres scores plus intéressants ou complémentaires (par exemple, Dunn et/ou l'indice de Davies-Bouldin), vous pouvez les appliquer en justifiant votre choix.

4. **Optimisation :**
   - Si nécessaire, réappliquez les algorithmes avec d'autres paramètres, par exemple, le DBSCAN avec d'autres paramètres, et recalculer les scores de silhouette. Gardez celui qui représente le meilleur score de silhouette.

5. **Analyse comparative :**
   - Comparez les performances des trois algorithmes sur le dataset choisi en utilisant les métriques calculées.
   - Analysez comment les performances varient en fonction des paramètres choisis et de l'algorithme utilisé.
   - D'après vous, quel est le meilleur algorithme et pourquoi ? (Résistance au bruit ? Forme des données ?)
   - Discutez des avantages et des inconvénients de chaque méthode pour la détection de chutes.

6. **Interprétation des résultats :**
   - Pour chaque méthode et paramètres, interprétez les clusters obtenus. Peuvent-ils être associés à des chutes ou à des activités normales ?
   - Discutez de la pertinence de l'approche non supervisée pour la détection de chutes.

7. **Rapport et présentation :**
   - Rédigez un rapport détaillant la méthodologie, les résultats et les conclusions.
   - Préparez une présentation visuelle des résultats les plus significatifs.

### Bonus :
   - Explorez d'autres méthodes de réduction de dimensionnalité (t-SNE, UMAP) pour la visualisation des clusters.
   - Proposez et implémentez une méthode pour déterminer automatiquement le nombre optimal de clusters pour K-means et le clustering hiérarchique.

### Citations :
1. [Machine Learning Clustering DBSCAN](https://datascientest.com/machine-learning-clustering-dbscan)
2. [Kaggle - Machine Learning Non Supervisé](https://www.kaggle.com/code/zoupet/machine-learning-non-supervis-correction)
3. [Principaux Algorithmes d'Apprentissage Non Supervisé](https://fr.linedata.com/principaux-algorithmes-dapprentissage-non-supervise)
4. [Apprentissage Non Supervisé de Flux de Données Massives](https://www.researchgate.net/publication/333772967_Apprentissage_non_supervise_de_flux_de_donnees_massives_application_aux_Big_Data_d%27assurance)
5. [Discovery Unsupervised Learning](https://fr.mathworks.com/discovery/unsupervised-learning.html)

---

Cet énoncé permet aux étudiants de travailler en profondeur sur différentes techniques de clustering, d'évaluer leur efficacité dans un contexte réel, et de développer leur capacité d'analyse et d'interprétation des résultats.
