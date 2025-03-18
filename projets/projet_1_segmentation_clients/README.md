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
  - **K-Means** : rapide et efficace, mais sensible aux valeurs aberrantes.
  - **DBSCAN** : détecte bien les **anomalies**, mais difficile à paramétrer.
  - **GMM** : utile pour des segments **chevauchants**, mais plus coûteux en calcul.

- **PySpark (MLlib)** :
  - **K-Means** : excellent pour les **grandes bases de données**.
  - **GMM** : utile pour des segments non linéaires.
  - **Bisecting K-Means** : alternative intéressante avec une meilleure **hiérarchisation** des clusters.





