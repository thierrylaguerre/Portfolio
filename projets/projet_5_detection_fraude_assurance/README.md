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
   - **Random forest**
   - **Régréssion logistique**
   - **Adaboost**

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
- **XGBoost (96% de précision)** : Meilleur compromis entre précision (0.94 pour la classe minoritaire) et rappel (0.78), offrant un bon équilibre.
- **Random Forest, SVM, ExtraTrees & Logistic Regression (94% de précision)** : Excellents résultats, mais le rappel sur la classe minoritaire (0.64) est un point d’amélioration.
- **KNN (90% de précision)** : Moins performant, mais un rappel plus élevé (0.78) pour la classe 1.
- **Adaboost (91% de précision)** : Performances acceptables, mais un rappel très faible (0.47) sur la classe 1, ce qui signifie qu’il manque de nombreuses détections.
- **Naive Bayes (30% de précision)** : Mauvaises performances globales, avec un rappel inversé (97% pour la classe 1 mais seulement 17% pour la classe 0), rendant le modèle inutilisable

