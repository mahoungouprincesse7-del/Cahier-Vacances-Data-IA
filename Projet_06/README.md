# 🍦 Projet 06 — Séries temporelles : combien de glaces préparer demain ?

## 🎯 Objectif

Aider un glacier de plage à **prévoir ses ventes du lendemain** à partir de 4 étés d'historique, en comparant des règles simples à des modèles statistiques **MA** et **ARMA**.

![Projet 06](projet_06.png)

## 📦 Données

- `ventes_glaces.csv` : **488 jours d'ouverture**, de juin 2022 à septembre 2025 (4 saisons d'été)
- Les **22 derniers jours** sont gardés comme jeu de test

## 🔎 Démarche

1. **Baselines** : « toujours prédire la moyenne » et « même chiffre qu'hier ».
2. **Autocorrélation** : codée à la main, puis corrélogrammes ACF / PACF → une journée ressemble fortement à la veille (r ≈ 0,81).
3. **Modèle MA(q)** : simulation d'un processus à moyenne mobile, puis estimation d'un MA(3) avec `statsmodels`.
4. **Modèle ARMA(1,1)** sur les 4 étés, comparé au MA(3) avec l'**AIC** et le test de **Ljung-Box** sur les résidus.
5. **Prévision à 7 jours** avec intervalle de confiance.

## 📊 Résultats (erreur moyenne sur les 22 jours de test)

| Modèle | Erreur moyenne (glaces / jour) |
|---|---:|
| **ARMA(1,1), 4 étés** | **14,80** |
| MA(3), 4 étés | 16,27 |
| MA(3), saison 2025 seule | 16,48 |
| « Comme hier » | 19,00 |
| « Toujours la moyenne » | 30,38 |

- L'ARMA(1,1) fait **mieux avec moins de coefficients** : AIC 3 920 contre 3 945 pour le MA(3).
- Ses résidus sont du bruit pur (Ljung-Box p = 0,59), alors que le MA(3) laisse de la structure non captée (p < 0,001).
- L'ARMA réduit l'erreur de **22 %** par rapport à la règle « comme hier ».

## 🛠️ Technologies

`Python` • `pandas` • `NumPy` • `statsmodels (ARIMA)` • `Matplotlib` • `ACF / PACF` • `AIC` • `Ljung-Box`

## 📁 Fichiers

- `Projet_06.ipynb` — notebook complet
- `utils.py` — fonctions de tracé et d'évaluation
- `data/ventes_glaces.csv` — données de ventes
