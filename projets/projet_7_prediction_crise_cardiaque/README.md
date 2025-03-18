# Projet 7 : Prédiction de crise cardiaque

## Description du projet

Ce projet vise à prédire la probabilité de survenue d'une crise cardiaque en fonction de plusieurs facteurs de risque. L'objectif est de construire un modèle de classification capable d'identifier les patients à risque élevé de crise cardiaque. Pour cela, nous utilisons des techniques d'analyse de données et des modèles de machine learning.

## Objectifs

- **Étudier les facteurs de risque** associés à la crise cardiaque.
- **Construire un modèle prédictif** capable d'estimer la probabilité qu'un patient fasse une crise cardiaque.
- **Évaluer les performances du modèle** en termes de précision et l'AUC-ROC.

## Structure du projet

````
projet_7_prediction_crise_cardiaque/
│── data/
│ ├── heart_attack_prediction_dataset.csv.zip # Dataset utilisé pour la prédiction
│── README.md # Documentation du projet
│── prediction_crise_cardiaque.ipynb # Notebook contenant l'implémentation du modèle
````

## Données

Le jeu de données utilisé dans ce projet contient des informations sur plusieurs variables liées à la santé des patients, telles que :

- Âge
- Sexe
- Taux de cholestérol
- Niveau de sucre sanguin
- Pression artérielle
- Historique familial de crise cardiaque, etc.

Les données sont fournies sous forme de fichier CSV compressé dans le répertoire `data/`.

## 🔧 Méthodologie

1. **Prétraitement des données** :
   - Nettoyage des données (suppression des valeurs manquantes, gestion des valeurs aberrantes).
   - Encodage des variables catégorielles (par exemple, le sexe).
   - Normalisation des données (scaling des variables numériques).

2. **Sélection des caractéristiques** :
   - Identification des principales variables influençant la prédiction de crise cardiaque.

3. **Modèles de Machine Learning** :
   - **Régression logistique** : Un modèle linéaire simple pour la classification binaire.
   - **Arbre de décision** : Un modèle non linéaire permettant une interprétation plus facile.
   - **Random Forest** : Un ensemble d'arbres de décision pour améliorer la robustesse du modèle.
   - **SVM (Support Vector Machine)** : Un modèle puissant pour la classification avec marges maximales.
   - **KNN (K-Nearest Neighbors)** : Un modèle de classification basé sur la proximité des points.
   - **Naive Bayes** : Un modèle probabiliste basé sur le théorème de Bayes.
   - **Perceptron** : Un modèle linéaire simple inspiré des neurones biologiques.

4. **Évaluation du modèle** :
   - Évaluation de la performance des modèles à l'aide des métriques suivantes : 
     - **Précision**
     - **AUC-ROC**

5. **Analyse et comparaison des performances des modèles** :
   - **Random Forest (63,6% de précsion)** : Meilleur modèle en termes de précision, mais l'AUC-ROC est faible, indiquant une capacité limitée à distinguer les classes.
   - **Decision Tree (54,5% de précision)**: Moins performant que Random Forest, avec une précision plus faible et un AUC-ROC également faible.
   - **Gaussian Naive Bayes (64,2% de précision)** : Bonne précision, mais l'AUC-ROC reste faible, ce qui signifie qu'il n'est pas très efficace pour classer les classes de manière discrète.
   - **Logistic Regression (64,2% de précision)** : Très similaire à Gaussian Naive Bayes en termes de précision et AUC-ROC, avec une bonne précision mais une faible capacité à séparer les classes.
   - **K-Nearest Neighbors (57,2% de précision)** : Précision plus faible et AUC-ROC également limité. Pas très performant sur cette tâche.
   - **Multi-Layer Perceptron (MLP) (56,2% de précision)** : Similaire à KNN et Decision Tree, avec une faible performance en termes de séparation des classes.
   - **SVM (0.642, AUC-ROC: 0.461)** : Précision correcte, mais l'AUC-ROC est faible, ce qui suggère que le modèle ne capture pas bien les différentes classes.

