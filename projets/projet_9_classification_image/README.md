# 🖼️ Projet 9 : Classification d'images

## 📊 Description du projet

Ce projet consiste à développer un modèle de classification d'images en utilisant des réseaux neuronaux convolutionnels (CNN). L'objectif est de classer un ensemble d'images en différentes catégories en fonction de leurs caractéristiques visuelles. Ce projet inclut le prétraitement des images, l'entraînement d'un modèle CNN et l'évaluation de la performance du modèle.

## 🎯 Objectifs

- **Prétraiter les images** pour les rendre adaptées à l'entraînement d'un modèle de machine learning.
- **Construire un modèle CNN** pour la classification d'images.
- **Évaluer la performance du modèle** en termes de précision, rappel et F1-score.

## 📂 Structure du projet

````
projet_9_classification_image/
│── data/
│ ├── (Dossier contenant les images à classer) # Les images sont stockées ici
│── README.md # Documentation du projet
│── classification_image.ipynb # Notebook contenant l'implémentation du modèle CNN
````

## 🖼️ Données

Les données utilisées dans ce projet comprennent un ensemble d'images provenant de différentes catégories (par exemple, animaux, objets, scènes, etc.). Les images sont fournies dans des dossiers séparés pour chaque catégorie, et chaque catégorie sera utilisée pour entraîner le modèle.

Les images sont fournies dans le répertoire `data/`.

## 🔧 Méthodologie

1. **Prétraitement des images** :
   - Redimensionnement des images à une taille fixe (par exemple, 128x128 pixels).
   - Normalisation des pixels (mise à l'échelle des valeurs de pixel entre 0 et 1).
   - Augmentation des données pour éviter le surapprentissage (par exemple, rotation, zoom, retournement horizontal).

2. **Modèle CNN** :
   - Développement d'un réseau neuronal convolutionnel (CNN) pour extraire des caractéristiques des images.
   - Architecture du modèle : couches de convolution, de pooling, de normalisation, et couches entièrement connectées (fully connected).
   - Fonction d'activation ReLU et fonction de perte basée sur l'entropie croisée.

3. **Entraînement du modèle** :
   - Entraînement du modèle CNN en utilisant les images d'entraînement et validation sur un ensemble de test pour évaluer la performance.
   - Optimisation du modèle à l'aide de techniques comme **Adam**.

4. **Évaluation du modèle** :
   - Évaluation de la performance du modèle sur l'ensemble de test en utilisant des métriques telles que :
     - **Précision**
     - **Rappel**
     - **F1-score**
   - Visualisation des courbes d'apprentissage pour observer la progression du modèle.

