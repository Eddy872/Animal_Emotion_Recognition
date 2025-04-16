# 🐾 Animal Emotion Classifier (Image Only)

Ce projet vise à entraîner un modèle de deep learning pour reconnaître l'émotion d'un animal à partir de **vidéos transformées en images** (frames).  
Le modèle prédit l'émotion parmi : `joy`, `fear`, `hunger`.

---

## 📁 Structure du dataset


- Les images sont nommées : `animal_emotion_id_frame.jpg`  
  Ex : `cat_fear_02_005.jpg`
- Le CSV contient 3 colonnes : `image`, `animal`, `emotion`

---

## ⚙️ Étapes du projet

1. 📽️ Extraction de frames depuis des vidéos `.mp4` classées par émotion
2. 📸 Génération du CSV à partir des noms de fichiers
3. 🧠 Entraînement d'un modèle CNN (TensorFlow) pour classer l'émotion
4. 📊 Affichage des courbes `accuracy` / `loss` et prédiction image par image

---

## 🧠 Modèle

Modèle CNN entraîné sur images redimensionnées à `224x224`.  
Optionnel : export vers Core ML (`.mlmodel`) pour usage iOS.

---