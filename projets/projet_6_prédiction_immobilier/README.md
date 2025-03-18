# Prédiction des Prix de l’Immobilier  

## Objectif du Projet  
L'objectif de ce projet est de **prédire les prix de l’immobilier** en fonction de plusieurs caractéristiques (superficie, nombre de chambres, localisation, etc.). Cette prédiction permet aux acheteurs, vendeurs et investisseurs d’avoir une meilleure estimation des prix du marché.

## Méthodologie  

1. **Analyse Exploratoire des Données (EDA)**  
   - Étude des tendances du marché immobilier.  
   - Visualisation des distributions des prix.  
   - Analyse de la corrélation entre les variables (superficie, localisation, etc.).  

2. **Prétraitement des Données**  
   - Suppression des **doublons et des valeurs manquantes**.  
   - Encodage des **variables catégorielles** (localisation, type de logement, etc.).  
   - **Normalisation et standardisation** des données.  
   - Séparation des données en **train/test**.  

3. **Modélisation & Entraînement des Modèles**  
   - **Régression Linéaire**  
   - **Lasso & Ridge Regression**  
   - **Random Forest Regressor**  
   - **XGBoost**  
   - **CatBoost**  

4. **Évaluation des Modèles**  
   - **Métriques utilisées** :  
     - Mean Absolute Error (MAE)  
     - Mean Squared Error (MSE)  
     - R² Score  

## 📂 Structure du Projet  

````
projet_6_prediction_immobilier/
│── data/
│ ├── real_estate_dataset.csv # Dataset des transactions immobilières
│── prediction_immobilier.ipynb # Notebook d’analyse et de modélisation
│── README.md # Présentation générale du projet
````

## 🚀 Résultats et Analyse  

### 📌 Comparaison des Modèles  
- **XGBoost & CatBoost** : Meilleurs résultats avec une faible erreur et un bon R².  
- **Régression Linéaire & Ridge** : Performances correctes, mais sensibles aux valeurs extrêmes.  
- **Random Forest** : Bonne précision mais temps d’entraînement plus long.  
 

---
