# 📊 Segmentation Client

## 📌 Objectif du projet
L’objectif de ce projet est de segmenter une base de clients afin d’identifier différents groupes aux comportements similaires. Cette segmentation permet aux entreprises d’optimiser leurs stratégies marketing et d’adapter leurs offres en fonction des besoins de chaque segment.

## 🔍 Méthodologie
1. **Préparation des données** : Nettoyage et transformation des données clients.
3. **Choix des méthodes de clustering** : Application des algorithmes de clustering :
   - **PySpark (MLlib)** → Scalabilité pour les grandes bases de données.
   - **Python (Scikit-learn)** → Comparaison des méthodes classiques.
4. **Évaluation des résultats** : Silhouette Score.
5. **Interprétation** : Identification des segments clés et recommandations.

## 📂 Structure du projet
```
projet_1_segmentation_clients/
│── pyspark/
│   ├── segmentation_pyspark.ipynb
│   ├── README.md  # Explication spécifique PySpark
│── python/
│   ├── segmentation_python.ipynb
│   ├── README.md  # Explication spécifique Python
│── data/  # Dataset utilisé pour tous
│── README.md  # Explication générale du projet
```

## 🚀 Résultats et Analyse
- 📌 **Comparaison des algorithmes** :
  - K-Means, DBSCAN et GMM ont été testés sur différentes plateformes.
  - **PySpark** est efficace pour traiter de gros volumes de données.
  - **Scikit-learn** offre une bonne flexibilité et des outils d’évaluation précis.

- 📊 **Interprétation des segments** :
  - Identification des profils clients dominants.
  - Définition de stratégies adaptées à chaque segment.



