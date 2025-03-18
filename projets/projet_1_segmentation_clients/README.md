# Segmentation de Clients avec PySpark et Python

## Objectif du projet
L’objectif de ce projet est de segmenter une base de clients en groupes distincts selon leurs comportements. Cette segmentation permet aux entreprises de **personnaliser leurs stratégies marketing** et d’optimiser leurs offres.

## Méthodologie

1. **Préparation des données**  
   - Gestion des **valeurs manquantes** et des **doublons**. 
   - Nettoyage et transformation des variables.

2. **Prétraitement des données**  
   - Encodage des **variables catégorielles**. 
   - Normalisation et **standardisation**.
   - Réduction de dimension avec **PCA**.

3. **Choix et entraînement des modèles de clustering**  
   - **Python (Scikit-learn)** :  
     - **K-Means**, **DBSCAN**, **GMM**.  
   - **PySpark (MLlib)** :  
     - **K-Means**, **GMM**, **Bisecting K-Means**.  

4. **Évaluation des performances**  
   - Utilisation de **Silhouette Score**.  


## Structure du projet
```
projet_1_segmentation_clients/
│── pyspark/
│   ├── segmentation_pyspark.ipynb
│── python/
│   ├── segmentation_python.ipynb
│── data/  # Dataset utilisé pour tous
|   ├── données_brutes.csv 
│── README.md  # Explication générale du projet
```

## Résultats et Analyse

### Comparaison des algorithmes
- **Python (Scikit-learn)** :
  - **K-Means** : le score de silhouette est 0.178148. Meilleur score parmi les trois algorithmes testés, mais reste faible, suggérant que les clusters ne sont pas bien séparés ou homogènes.
  - **DBSCAN** : le score de silhouette est 0.100885. Un score intermédiaire, mais toujours faible, peut-être à cause d'un mauvais choix des paramètres 
  - **GMM** : le score de silhouette est 0.017620. Très faible score, indiquant probablement un mauvais regroupement avec des clusters peu distincts.


- **PySpark (MLlib)** :
  - **K-Means** : le score de silhouette est 0.5708954149193984. Offre la meilleure séparation des clusters, indiquant une structure bien définie dans les données.
  - **GMM** : le score de silhouette est 0.2052461813447454. Produit des clusters moins distincts, suggérant qu’il ne capture pas bien la structure des données.
  - **Bisecting K-Means** : le score de silhouette est 0.5632952501029738. Très proche de K-Means, il segmente efficacement les données avec une approche hiérarchique.





