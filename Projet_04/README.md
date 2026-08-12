# 🤖 Projet 04 — Assistant IA RAG pour un hôtel

## 🎯 Objectif

Construire un assistant capable de répondre aux questions des clients d'un hôtel à partir de sa documentation interne, tout en limitant les hallucinations du modèle de langage.

## 🔎 Problèmes résolus

- Tester les limites d'un LLM lorsqu'il répond sans documentation.
- Extraire et nettoyer les informations contenues dans plusieurs fichiers PDF.
- Structurer la documentation de l'hôtel en sections utilisables par le modèle.
- Construire des prompts imposant au LLM de répondre uniquement à partir des informations disponibles.
- Transformer les différentes rubriques en **embeddings**.
- Comparer les textes grâce à la **similarité cosinus**.
- Mettre en place une recherche sémantique pour retrouver automatiquement les pages les plus pertinentes.
- Construire un pipeline **RAG** :
  question → recherche documentaire → contexte pertinent → LLM → réponse.
- Retourner les sources utilisées avec la réponse.
- Réduire la quantité de documentation envoyée au modèle et améliorer la rapidité des réponses.

## 🧠 Compétences

`Python` • `Hugging Face Transformers` • `Sentence Transformers` • `RAG` • `LLM` • `Embeddings` • `Recherche sémantique` • `Similarité cosinus` • `PyPDF` • `Pandas` • `NumPy` • `t-SNE`