# Prédiction des Ventes Commerciales en Fonction des Investissements Publicitaires

## Objectif du Projet
L'objectif de ce projet est de prédire les **ventes commerciales** en fonction des investissements réalisés dans différents médias (**TV, Radio, Journaux**). Cette analyse permet d'optimiser les **stratégies publicitaires** et d’identifier les canaux les plus rentables.

## Méthodologie

1. **Analyse Exploratoire des Données (EDA)**
   - Visualisation des relations entre les investissements publicitaires et les ventes.
   - Identification des **corrélations** entre les variables.
   - Détection des **valeurs aberrantes**.

2. **Prétraitement des Données**
   - **Suppression des doublons et des valeurs manquantes**.
   - **Normalisation et standardisation** pour améliorer la performance de certains modèles.
   - Séparation en **train/test** pour l'entraînement et l'évaluation.

3. **Entraînement des Modèles de Machine Learning**
   - **Régression Linéaire**  
   - **Arbre de Décision**  
   - **Random Forest**  
   - **Support Vector Regression (SVR)**  
   - **K-Nearest Neighbors (KNN)**  
   - **XGBoost**  

4. **Évaluation des Modèles**
   - Comparaison des modèles à l’aide des métriques suivantes :
     - **MSE (Mean Squared Error)**
     - **RMSE (Root Mean Squared Error)**
     - **R² Score**  

   
## Structure du Projet

```
projet_2_prediction_ventes_pub/
│── data/
│ ├── Advertising Budget and Sales.csv # Données 
│── regression_python.ipynb # Notebook d'analyse et de modélisation
│── README.md # Présentation générale du projet
````

## Résultats et Analyse

### Comparaison des Algorithmes
- **Random Forest :** Meilleur modèle avec une **MAE de 0.68**, un **R² de 0.98** et une **accuracy de 98%**, indiquant une excellente prédiction.
- **XGBoost :** Performant mais légèrement en dessous de Random Forest, avec un **R² de 0.97** et une **accuracy de 97%**.
- **Decision Tree :** Moins précis, avec un **R² de 0.92** et une **accuracy de 92%**, montrant une perte de performance par rapport aux ensembles.
- **Régression Linéaire :** Performances limitées **(R² de 0.89)**, suggérant que les relations ne sont pas purement linéaires.
- **KNN :** Similaire à la régression linéaire **(R² de 0.89)**, peut être sensible aux valeurs aberrantes.
- **SVR :** Résultats **proches de KNN et de la régression linéaire**, mais moins performant que les modèles ensemblistes.




