# 🚴 Projet 03 — Optimisation du Tour de France 2027

## 🎯 Objectif

Construire un tracé optimisé du Tour de France 2027 à partir de **120 villages**, en les répartissant en **21 étapes géographiquement cohérentes**, puis en recherchant le meilleur ordre de passage dans chaque étape.

## 🔎 Problèmes résolus

- Analyse de la répartition géographique des 120 villages.
- Conversion des coordonnées GPS pour travailler avec des distances réalistes.
- Création de 21 étapes par **clustering non supervisé**.
- Comparaison de **K-Means** et de la **Classification Ascendante Hiérarchique (CAH)** avec le score de silhouette.
- Sélection du modèle en combinant métriques statistiques et contraintes métier.
- Calcul des distances entre villages avec la formule de **Haversine**.
- Construction d'une matrice de distances 120 × 120.
- Résolution approchée du problème du voyageur de commerce (**TSP**).
- Construction des parcours avec un **algorithme glouton (Nearest Neighbor)**.
- Amélioration des parcours avec l'algorithme **2-opt**.
- Optimisation des 21 étapes en testant plusieurs villages de départ.
- Réduction d'un parcours naïf d'environ **47 000 km à environ 4 000 km**.

## 🧠 Compétences

`Python` • `Pandas` • `Scikit-learn` • `K-Means` • `Clustering hiérarchique` • `Silhouette Score` • `Haversine` • `TSP` • `Greedy Algorithm` • `2-opt` • `Matplotlib`