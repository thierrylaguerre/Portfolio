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

### Comparaison des Modèles  

- **Régression Linéaire & LASSO (97.09% de précision)** : Excellentes performances avec un **R² de 0.97** et une **précision proche de 97%**. Ces modèles sont adaptés pour des prédictions précises et simples.
- **Ridge (97.06% de précision)** : Très proche de la régression linéaire et du LASSO, offrant des performances similaires mais avec une régularisation légèrement différente.
- **CatBoost (91.94% de précision)** : Bon modèle avec une **précision de 91.94%**, mais le R² est plus bas (0.92), indiquant qu'il peut y avoir des zones d’amélioration.
- **XGBoost (84.43% de précision)** : Moins performant que CatBoost, mais tout de même solide avec un **R² de 0.84**. Un peu plus complexe à optimiser mais utile pour des ensembles de données plus complexes.
- **Random Forest (82.44%)** : Précision encore plus faible avec un **R² de 0.82**, indiquant que les prédictions ne sont pas aussi fines que celles des modèles précédents.
- **K-NN (69.91% de précision)** : Le moins performant avec une **précision de 69.91%** et un **R² de 0.70**, suggérant que les voisins peuvent ne pas être une bonne approche pour cette tâche. 

---
