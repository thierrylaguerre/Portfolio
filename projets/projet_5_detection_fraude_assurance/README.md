# Détection de Fraude en Assurance  

## Objectif du Projet  
L'objectif de ce projet est de **détecter les fraudes en assurance** en analysant les demandes d’indemnisation afin d’identifier les comportements suspects. Une meilleure détection permet aux compagnies d'assurance de **réduire les pertes financières** et d’**améliorer leur gestion des risques**.

## Méthodologie  

1. **Analyse Exploratoire des Données (EDA)**  
   - Étude des caractéristiques des **demandes d'indemnisation**.  
   - Identification des **patterns suspects** dans les données.  
   - Détection des déséquilibres de classes (fraude vs non-fraude).  

2. **Prétraitement des Données**  
   - Suppression des **doublons** et des **valeurs manquantes**.  
   - **Encodage des variables catégorielles**.  
   - **Normalisation et standardisation** des données pour certains modèles.  

3. **Gestion du Déséquilibre des Classes**  
   - Techniques de **sous-échantillonnage (undersampling)** et de **sur-échantillonnage (SMOTE)** pour équilibrer les classes.  

4. **Modélisation & Entraînement des Modèles**  
   - **Random Forest**  
   - **XGBoost**  
   - **Gradient Boosting**  
   - **K-Nearest Neighbors (KNN)**  
   - **Naive Bayes**  

5. **Évaluation des Modèles**  
   - **Métriques utilisées** :  
     - Accuracy  
     - Precision  
     - Recall  
     - F1-score  
     - AUC-ROC  

## Structure du Projet  
````
projet_5_detection_fraude_assurance/
│── data/
│ ├── fraud_oracle.csv.zip # Dataset des demandes d'indemnisation
│── detection_fraude_assurance.ipynb # Notebook d'analyse et de modélisation
│── README.md # Présentation générale du projet
````


## Résultats et Analyse  

### Comparaison des Modèles  
- **Random Forest & XGBoost** : Meilleurs résultats en précision et en rappel.  
- **Gradient Boosting** : Bonne performance, mais plus lent à entraîner.  
- **KNN & Naive Bayes** : Moins performants sur ce jeu de données.  


