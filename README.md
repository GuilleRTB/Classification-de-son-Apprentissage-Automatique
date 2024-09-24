# Classification des Sons Cardiaques à l'Aide de Techniques d'Apprentissage Supervisé et Non Supervisé

## Introduction

Ce projet vise à exploiter l'intelligence artificielle (IA) pour l'analyse des sons cardiaques dans le cadre du diagnostic médical. Plus précisément, nous analysons trois types distincts de sons cardiaques : les battements normaux, les murmures et les artefacts. Ces sons sont transformés en paramètres exploitables grâce à la conversion des enregistrements audio en Coefficients Céphalométriques de Fréquence de Mel (MFCC) à l'aide de la bibliothèque Python librosa. Cette approche permet d'extraire les caractéristiques fréquentielles essentielles des enregistrements pour une analyse plus précise.

Nous utilisons à la fois des méthodes d'apprentissage supervisé et non supervisé pour classifier ces sons cardiaques. L'objectif final est de développer un modèle performant capable d'identifier les anomalies cardiaques avec précision.

## Structure du Projet

### Pré-traitement des données :

- Conversion des sons en coefficients MFCC avec librosa.
- Analyse exploratoire des données (EDA) pour visualiser les distributions des MFCC via des histogrammes et boîtes à moustaches.

### Modèles de Classification :

- **Random Forest** : Construction d'une forêt d'arbres de décision pour la classification des sons.
- **Support Vector Machines (SVM)** : Utilisation de SVM avec noyau RBF pour séparer les classes non linéaires.
- **k-Nearest Neighbors (k-NN)** : Classification basée sur les voisins les plus proches.

### Évaluation des Modèles :

- Visualisation des performances avec des courbes d'exactitude et de précision.
- Optimisation des hyperparamètres (profondeur maximale des arbres, nombre de voisins, etc.).
- Matrices de confusion pour évaluer les erreurs de classification par classe.