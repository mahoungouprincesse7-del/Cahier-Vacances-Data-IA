# Projet 01 — Analyse SQL d'une base de réservations aériennes ✈️

## 🎯 Objectif

Utiliser **SQL** pour analyser les données de vols, passagers et réservations d'un aéroport et répondre à une problématique métier :

> **Quelle destination déjà desservie renforcer avec un vol hebdomadaire supplémentaire, et quels clients cibler en priorité ?**

## 🔎 Analyses réalisées

- Recherche et filtrage des **vols au départ de Nice** et des offres à moins de **100 €**.
- Analyse des réservations : **confirmées, annulées et en attente**.
- Calcul du **chiffre d'affaires par destination** et identification des destinations avec une demande récurrente.
- Identification de **New York JFK** comme destination la plus intéressante à renforcer.
- Analyse des passagers du vol **AF5501 Nice → New York**, de leur classe et de leur siège.
- Comparaison du **prix des vols avec le prix moyen** pour étudier le positionnement premium de New York.
- Identification des **clients sans réservation** pour de futures campagnes marketing.
- Identification des **clients fidèles ayant au moins deux réservations** afin de leur proposer les nouveaux billets en priorité.

## 📊 Résultat

L'analyse conduit à recommander le renforcement de la liaison vers **New York JFK**, avec un ciblage prioritaire des **clients fidèles** pour le lancement des nouveaux billets.

## 🛠️ Technologies et compétences

**Technologies :**

`SQL` • `SQLite` • `Python` • `Pandas` • `Jupyter Notebook`

**SQL :**

`SELECT` • `WHERE` • `ORDER BY` • `GROUP BY` • `HAVING` • `JOIN` • `COUNT` • `SUM` • `AVG` • Sous-requêtes

## 📁 Fichiers

- `projet_01.ipynb` — notebook contenant l'analyse complète
- `base_de_données.png` — schéma de la base de données