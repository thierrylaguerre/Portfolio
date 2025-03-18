# Projet 8 : Système de recommandation

## Description du projet

Ce projet consiste à implémenter un système de recommandation basé sur le filtrage de contenu pour recommander des films aux utilisateurs en fonction de leurs préférences. L'idée est de prédire quels films un utilisateur pourrait apprécier, en se basant sur les caractéristiques des films qu'il a déjà regardés et appréciés.

## Objectifs

- **Analyser les données** de films et d'utilisateurs pour extraire des caractéristiques pertinentes.
- **Implémenter un système de recommandation** basé sur le filtrage de contenu.
- **Évaluer la performance du système** à l'aide de métriques de recommandation.

## Structure du projet

````
projet_8_système_recommandation/
│── data/
│ ├── movies.csv.zip # Dataset contenant les informations sur les films
│── README.md # Documentation du projet
│── film_recommandation.ipynb # Notebook contenant l'implémentation du système de recommandation
````

## Données

Le dataset utilisé dans ce projet contient des informations sur les films, telles que :

- Titre du film
- Genres (par exemple, Action, Comédie, Drame, etc.)
- Description du film
- Année de sortie
- Autres caractéristiques des films (par exemple, les mots-clés associés)

Les données sont fournies sous forme de fichier CSV compressé dans le répertoire `data/`.

## Méthodologie

1. **Prétraitement des données** :
   - Nettoyage des données (suppression des valeurs manquantes et gestion des doublons).
   - Tokenisation et vectorisation des genres et des descriptions des films.

2. **Filtrage de contenu** :
   - Calcul de la similarité entre les films en utilisant des techniques comme le **TF-IDF** (Term Frequency-Inverse Document Frequency) pour les descriptions textuelles et les genres.
   - Calcul de la similarité entre les films en utilisant la **similarité cosine**.

3. **Recommandation de films** :
   - Basé sur les films similaires, recommander les films les plus pertinents pour un utilisateur donné.
   - Affichage des films recommandés en fonction des caractéristiques des films préférés de l'utilisateur.

4. **Évaluation du système** :
   - Évaluation de la pertinence des recommandations à l'aide de métriques comme le **Mean Average Precision** (MAP) et le **Hit Rate**.


