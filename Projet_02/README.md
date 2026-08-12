# ⚽ Projet 02 — Prédiction de matchs de football avec Machine Learning

## Objectif

Analyser plus de 30 000 matchs internationaux de l'ère moderne (1994–2026) et construire un modèle capable d'estimer le vainqueur d'un match à partir de la forme récente des équipes.

## Problématiques étudiées

- Mesurer l'avantage de jouer à domicile.
- Identifier les équipes ayant remporté le plus de matchs depuis 1994.
- Étudier l'évolution du nombre moyen de buts par match.
- Calculer la forme récente des équipes à partir de leurs derniers matchs.
- Construire des variables comparant les performances des deux adversaires.
- Entraîner et évaluer un modèle de classification Random Forest.
- Prédire le vainqueur d'une rencontre et sa probabilité de victoire.
- Simuler un tournoi complet à élimination directe jusqu'au champion.

## Méthodes utilisées

- Analyse exploratoire avec Pandas
- Feature engineering
- Standardisation avec StandardScaler
- RandomForestClassifier
- Classification binaire
- Évaluation avec l'accuracy
- Simulation de matchs avec `predict_proba`

## Technologies

Python · Pandas · NumPy · Matplotlib · Scikit-learn