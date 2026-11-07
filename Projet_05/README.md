# 🐠 Projet 05 — Détection de poissons par Deep Learning (Faster R-CNN)

## 🎯 Objectif

Construire un détecteur capable d'**encadrer et de nommer les poissons** présents sur une photo d'aquarium, en adaptant un modèle de vision pré-entraîné à 13 espèces.

![Projet 05](image.png)

## 📦 Données

- Dataset Kaggle **Fish Dataset** : **7 750 photos étiquetées** (boîtes englobantes + espèce)
- **13 espèces** : AngelFish, BlueTang, ButterflyFish, ClownFish, GoldFish, Gourami, MorishIdol, PlatyFish, RibbonedSweetlips, ThreeStripedDamselfish, YellowCichlid, YellowTang, ZebraFish
- Classes déséquilibrées (de 142 à plus de 800 photos selon l'espèce)

## 🔎 Démarche

1. **Constat de départ** : le Faster R-CNN pré-entraîné sur COCO ne connaît aucune catégorie « poisson » → il détecte un poisson-clown comme un *bird* (oiseau) à 98 %.
2. **Préparation des données** : `Dataset` et `DataLoader` PyTorch, images 640×640 normalisées, conversion des boîtes et des labels.
3. **Fine-tuning** (*transfer learning*) : remplacement de la tête de classification pour 13 espèces + fond, 14,6 M de paramètres entraînables sur 19 M.
4. **Entraînement** sur 1 000 photos (validation sur 300) : la loss passe de **0,78 à 0,64** en 2 epochs.
5. **Test** : le même poisson est maintenant reconnu comme **ClownFish à 98 %**, avec sa boîte.

## 📊 Résultat

| Modèle | Prédiction sur la même photo |
|---|---|
| Faster R-CNN pré-entraîné (COCO) | ❌ `bird` (0,98) |
| Faster R-CNN fine-tuné | ✅ `ClownFish` (0,98) |

## 🛠️ Technologies

`Python` • `PyTorch` • `torchvision` • `Faster R-CNN (MobileNetV3)` • `Transfer learning` • `torchmetrics` • `kagglehub` • `Google Colab (GPU)`

## 📁 Fichiers

- `projet_05.ipynb` — notebook complet
- `utils.py` — fonctions d'affichage et de chargement
- `ma_photo_aquarium.jpg` — photo personnelle testée avec le détecteur
