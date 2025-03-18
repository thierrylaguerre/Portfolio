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
- **Logistic Regression & SVM** : Les meilleurs modèles en termes de **précision avec 85%**, indiquant une bonne capacité de classification.
- **GRU** : **Précision de 84%**. Très proche des meilleurs, ce qui montre que ce réseau de neurones récurrent capte bien les dépendances temporelles.
- **CNN** : **Précision de 82%**. Performant, surtout si les données ont une structure spatiale exploitable.
- **Naive Bayes** : **Précision de 81%**. Solide, surtout si les données respectent l’hypothèse d’indépendance conditionnelle.
- **Random Forest** : **Précision de 80%**. Légèrement en dessous des autres modèles, peut-être dû à des données non adaptées aux arbres de décision.
- **LSTM** : **Précision de 22%**. Très faible, suggérant un problème d’apprentissage (sous-apprentissage, manque de données, mauvais hyperparamètres).
---

