# 📊 Segmentation Client - PySpark

## 📌 Objectif de l'implémentation PySpark
L’objectif de cette version est d’implémenter la segmentation client en utilisant **PySpark MLlib**, qui permet de traiter de grandes bases de données efficacement grâce à la parallélisation.

## 🔍 Méthodologie
1. **Chargement des données** : Utilisation de `données_brute.csv` pour lire et manipuler les données.
2. **Prétraitement** : Nettoyage et transformation des données avec `VectorAssembler` et `StandardScaler`.
3. **Modélisation** :
   - **K-Means** : Clustering basé sur la minimisation de la variance intra-cluster.
   - **Bisecting K-Means** : Variante hiérarchique de K-Means pour une meilleure séparation des clusters.
   - **GMM (Gaussian Mixture Model)** : Segmentation basée sur une distribution probabiliste des clusters.
4. **Évaluation des modèles** : Calcul du **Silhouette Score** et analyse des résultats.
5. **Visualisation** : Utilisation de `matplotlib` et `seaborn` après extraction des données de Spark.

## 📂 Contenu du répertoire PySpark
```
pyspark/
│── segmentation_pyspark.ipynb  # Notebook avec l'implémentation complète
│── README.md  # Explication spécifique PySpark
```

## 🚀 Avantages de PySpark
✅ **Scalabilité** : Adapté aux grands jeux de données.  
✅ **Rapidité** : Traitement distribué pour des calculs plus rapides.  
✅ **Intégration facile** : Compatible avec les environnements Big Data.  

## 📊 Résultats et Analyse
- **Performance** : Comparaison des scores de clustering pour différentes configurations.
- **Interprétation** : Identification des groupes de clients et de leurs caractéristiques dominantes.

