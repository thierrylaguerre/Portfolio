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

- **Isolation Forest**.
- **Régression Logistique**.
- **XGBoost**.
- **Random Forest**.
- **Hist Gradient Boosting**.

### 4. **Comparaison des Performances des Modèles**

Une fois les modèles entraînés, leurs performances ont été comparées à l’aide de plusieurs métriques, telles que :

- **AUC (Area Under the Curve)**
- **Précision**
- **Rappel**
- **Score F1**
- **Matrice de confusion**

Cette évaluation a permis de sélectionner le modèle le plus efficace pour la détection de fraude.

---



