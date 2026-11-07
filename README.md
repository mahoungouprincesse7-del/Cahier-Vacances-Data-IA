# 🏖️ Cahier de vacances Data & IA — 6 projets en 2026

Série de mini-projets réalisés pendant l'été 2026 dans le cadre du **Cahier de vacances [Machine Learnia](https://github.com/MachineLearnia/Cahier-Vacances-2026)**. Chaque semaine, un projet complet : de l'analyse SQL au Deep Learning, en passant par le Machine Learning, l'optimisation, les LLM et les séries temporelles.

## 📚 Les projets

| # | Projet | Ce que j'ai fait | Résultat clé | Outils |
|---|---|---|---|---|
| 01 | [✈️ Analyse SQL de réservations aériennes](Projet_01) | Requêtes SQL pour choisir une destination à renforcer et les clients à cibler | Recommandation : renforcer **New York JFK** et cibler les clients fidèles | SQL, SQLite, pandas |
| 02 | [⚽ Prédiction de matchs de football](Projet_02) | +30 000 matchs internationaux, feature engineering sur la forme récente, simulation de tournoi | Accuracy **65,4 %** sur 4 412 matchs de test (vs 62,7 % en prédisant toujours l'équipe à domicile) | scikit-learn, pandas |
| 03 | [🚴 Optimisation du Tour de France 2027](Projet_03) | Clustering de 120 villages en 21 étapes, puis optimisation des parcours (TSP) | Parcours réduit de **~47 000 km à ~4 000 km** | K-Means, CAH, 2-opt |
| 04 | [🤖 Assistant IA RAG pour un hôtel](Projet_04) | Pipeline RAG sur 5 PDF : embeddings, recherche sémantique, réponses sourcées | Assistant qui répond uniquement à partir de la documentation | Hugging Face, Sentence Transformers, LLM |
| 05 | [🐠 Détection de poissons](Projet_05) | Fine-tuning d'un Faster R-CNN sur 7 750 photos et 13 espèces | De `bird` (erreur) à `ClownFish` à 98 % | PyTorch, torchvision |
| 06 | [🍦 Prévision des ventes de glaces](Projet_06) | Autocorrélation, modèles MA et ARMA, prévision à 7 jours | Erreur réduite de **22 %** vs « comme hier » | statsmodels |

## 🧠 Compétences mobilisées

- **Données** : SQL, pandas, NumPy, nettoyage et feature engineering
- **Machine Learning** : classification (Random Forest), clustering (K-Means, CAH), score de silhouette
- **Deep Learning** : PyTorch, transfer learning, détection d'objets
- **IA générative** : LLM, embeddings, RAG
- **Statistiques** : séries temporelles (MA, ARMA), AIC, tests sur les résidus
- **Optimisation** : problème du voyageur de commerce, algorithme glouton, 2-opt

## ▶️ Lancer les notebooks

```bash
git clone https://github.com/mahoungouprincesse7-del/Cahier-Vacances-Data-IA.git
cd Cahier-Vacances-Data-IA
uv sync
```

Puis ouvrir le notebook du projet souhaité (`Projet_0X/projet_0X.ipynb`) dans Jupyter ou VS Code. Le Projet 05 nécessite un GPU (réalisé sur Google Colab).

---

👩‍💻 **Princesse Mahoungou** — M1 Modélisation des données, Université de Lille · [LinkedIn](https://www.linkedin.com/in/mahoungou-princesse-74509a2a0)
