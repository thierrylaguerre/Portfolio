# Détection de Fraude par Carte de Crédit

## Description du projet

Ce projet a pour objectif de détecter les fraudes potentielles sur des transactions effectuées par carte de crédit à l'aide de l'apprentissage automatique. Les données utilisées sont basées sur un ensemble de transactions financières, où l'objectif est de classer les transactions comme frauduleuses ou légitimes.

## Étapes du projet

### 1. **Analyse Exploratoire des Données (EDA)**

L'EDA a été réalisée pour mieux comprendre les données et en explorer les caractéristiques importantes. Cela inclut la visualisation des distributions, l'analyse des tendances et l'examen des corrélations entre les variables.

- **Visualisation des variables** : distribution des montants des transactions, répartition des transactions frauduleuses vs légitimes.
- **Identification des anomalies** : détecter les outliers ou valeurs extrêmes qui pourraient indiquer des anomalies dans les transactions.

### 2. **Prétraitement des Données**

Le prétraitement des données est une étape cruciale dans ce projet. Plusieurs opérations ont été effectuées pour garantir que les données soient prêtes pour l'entraînement des modèles.

- **Suppression des doublons** : élimination des transactions dupliquées dans le jeu de données.
- **Gestion des valeurs manquantes** : les valeurs manquantes ont été traitées en les supprimant ou en les imputant, selon le cas.
- **Normalisation et standardisation des données** : les caractéristiques numériques ont été normalisées pour garantir que les modèles puissent apprendre efficacement sans que certaines variables dominent les autres.
- **Encodage des variables catégorielles** : les variables catégorielles ont été encodées en valeurs numériques à l’aide de techniques comme l’encodage One-Hot ou Label Encoding.
- **Gestion du déséquilibre des classes avec SMOTE (Synthetic Minority Over-sampling Technique)** : Le déséquilibre entre les classes (frauduleuses vs légitimes) a été atténué en générant de nouvelles instances pour la classe minoritaire à l’aide de la méthode SMOTE.

### 3. **Entraînement et Évaluation des Modèles**

Plusieurs modèles ont été utilisés et évalués pour identifier celui qui offre les meilleures performances pour la détection de fraude.

- **Isolation Forest** : Un algorithme basé sur l'isolement des observations pour détecter les anomalies.
- **Régression Logistique** : Un modèle classique pour des problèmes de classification binaire.
- **XGBoost** : Un modèle de boosting très performant, adapté aux problèmes de classification sur des données tabulaires.
- **Random Forest** : Un algorithme d’ensemble utilisant plusieurs arbres de décision pour améliorer la précision.
- **Hist Gradient Boosting** : Un algorithme de gradient boosting basé sur des histogrammes pour gérer efficacement des grands volumes de données.

### 4. **Comparaison des Performances des Modèles**

Une fois les modèles entraînés, leurs performances ont été comparées à l’aide de plusieurs métriques, telles que :

- **AUC (Area Under the Curve)**
- **Précision**
- **Rappel**
- **Score F1**
- **Matrice de confusion**

Cette évaluation a permis de sélectionner le modèle le plus efficace pour la détection de fraude.

## Compétences et Technologies Utilisées

- **Hist Gradient Boosting**
- **Gestion des données** : Nettoyage, transformation et prétraitement des données.
- **Frameworks de Deep Learning** : TensorFlow, Keras (pour des modèles plus avancés si nécessaire).
- **Forêt Aléatoire** : Random Forest pour des classifications robustes.
- **Apprentissage Automatique** : Régression logistique, XGBoost, Isolation Forest pour des approches variées de la classification.
- **SMOTE** : Gestion du déséquilibre des classes pour améliorer les performances de détection de fraudes.

## Installation

1. **Cloner le dépôt** :

```bash
git clone https://github.com/votre-utilisateur/detection-fraude-cartes.git

````

Installer les dépendances :
```bash
pip install -r requirements.txt
````
Exécution du projet :
Lancer le script principal pour effectuer les analyses et l’entraînement des modèles :

`````bash
python main.py
``````

# Conclusion
Ce projet de détection de fraude par carte de crédit met en évidence l'importance de la préparation des données et de l'évaluation de plusieurs modèles afin de garantir des résultats optimaux. Les techniques utilisées, telles que SMOTE pour la gestion du déséquilibre et l'utilisation de plusieurs modèles d'apprentissage automatique, ont permis d'améliorer la détection des fraudes.

