# 🚑 Projet 7 : Prédiction de crise cardiaque

## 📊 Description du projet

Ce projet vise à prédire la probabilité de survenue d'une crise cardiaque en fonction de plusieurs facteurs de risque. L'objectif est de construire un modèle de classification capable d'identifier les patients à risque élevé de crise cardiaque. Pour cela, nous utilisons des techniques d'analyse de données et des modèles de machine learning.

## 🧑‍⚕️ Objectifs

- **Étudier les facteurs de risque** associés à la crise cardiaque.
- **Construire un modèle prédictif** capable d'estimer la probabilité qu'un patient fasse une crise cardiaque.
- **Évaluer les performances du modèle** en termes de précision, rappel et F1-score.

## 📂 Structure du projet

````
projet_7_prediction_crise_cardiaque/
│── data/
│ ├── heart_attack_prediction_dataset.csv.zip # Dataset utilisé pour la prédiction
│── README.md # Documentation du projet
│── prediction_crise_cardiaque.ipynb # Notebook contenant l'implémentation du modèle
````

## 📊 Données

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
     - **Rappel**
     - **F1-score**
     - **Matrice de confusion**

5. **Analyse et comparaison des performances des modèles** :

