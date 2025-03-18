# Analyse de Sentiments des Avis des Visiteurs des Parcs Disneyland  

## Objectif du Projet  
L'objectif de ce projet est d'analyser et de classifier les **avis des visiteurs des parcs Disneyland** afin de comprendre leurs **sentiments** (positifs, négatifs ou neutres). Cette analyse permet d’identifier les **points d’amélioration** pour l’expérience client.

## Méthodologie  

1. **Analyse Exploratoire des Données (EDA)**  
   - Visualisation de la **distribution des notes** attribuées par les visiteurs.  
   - Analyse de la **longueur des avis** et de leur répartition.  
   - Identification des tendances générales.  

2. **Prétraitement des Données**  
   - Suppression des **doublons** et des **valeurs manquantes**.  
   - Nettoyage des avis : **suppression des caractères spéciaux** et des **stopwords**.  
   - Conversion des avis en **minuscule** pour uniformisation.  

3. **Natural Language Processing (NLP)**  
   - **Tokenization** : découpage du texte en mots.  
   - **Stemming** : réduction des mots à leur racine pour limiter la diversité des termes.  

4. **Entraînement des Modèles de Machine Learning et Deep Learning**  
   - **Logistic Regression**  
   - **Support Vector Machine (SVM)**  
   - **Random Forest**  
   - **Naive Bayes**  
   - **LSTM (Long Short-Term Memory)**  
   - **CNN (Convolutional Neural Network)**  
   - **GRU (Gated Recurrent Unit)**  

5. **Évaluation des Performances des Modèles**  
   - Comparaison des modèles à l’aide de métriques comme :  
     - **Accuracy**  
     - **F1-score**  
     - **Recall & Precision**  

## 📂 Structure du Projet  

````
projet_3_analyse_sentiments/
│── data/
│ ├── DisneylandReviews.csv.zip # Dataset des avis des visiteurs
│── projet_analyses_sentiments.ipynb # Notebook d'analyse et de modélisation
│── README.md # Présentation générale du projet
````

## Résultats et Analyse  

### Comparaison des Modèles  
- **Logistic Regression & SVM** : Simples et performants pour les petits jeux de données.  
- **Random Forest** : Robuste mais nécessite plus de données pour une meilleure précision.  
- **Naive Bayes** : Rapide mais moins performant sur des textes longs et variés.  
- **LSTM, CNN & GRU** : Meilleurs résultats en Deep Learning, mais nécessitent **beaucoup de données et de ressources**.  
---

