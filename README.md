# Génération Automatique de Légendes d'Images  

Ce projet vise à développer un système innovant de génération automatique de légendes d'images en exploitant les techniques avancées de **deep learning**, **vision par ordinateur**, et **traitement du langage naturel (NLP)**.  

---

## 📋 Table des Matières  
- [Aperçu](#aperçu)  
- [Principales Fonctionnalités](#principales-fonctionnalités)  
- [Technologies Utilisées](#technologies-utilisées)  
- [Pipeline de Travail](#pipeline-de-travail)  
  - [Phase 1 : Classification d'Images](#phase-1--classification-dimages)  
  - [Phase 2 : Génération de Légendes](#phase-2--génération-de-légendes)  
  - [Phase 3 : Déploiement Web](#phase-3--déploiement-web)  
- [Démo](#démo)   

---

## 🔍 Aperçu  
Développé dans le cadre de ma formation en **Génie Logiciel**, ce projet comprend trois phases clés :  
1. **Classification d'Images** : Classification d'images en catégories telles que photographies, peintures, schémas et croquis grâce à **Vision Transformer (ViT)**.  
2. **Génération de Légendes** : Génération automatique de descriptions pertinentes à partir d'images grâce à une architecture **Encodeur-Décodeur Transformer** et des techniques NLP avancées.  
3. **Déploiement Web** : Développement d'une interface web intuitive avec **Flask** pour tester le système complet en temps réel.  

---

## 🌟 Principales Fonctionnalités  
- Classification précise d'images grâce à des modèles de deep learning avancés.  
- Génération automatique de légendes avec un modèle Transformer.  
- Application web conviviale pour tester le système en temps réel.  

---

## 🛠️ Technologies Utilisées  
- **Python** : Langage principal  
- **PyTorch** : Construction et entraînement des modèles  
- **Vision Transformer (ViT)** : Classification d'images  
- **Encodeur-Décodeur Transformer** : Génération de légendes  
- **Flask** : Développement de l'application web  
- **Outils NLP & LLM** : BLEU, CIDEr, METEOR pour évaluer les performances  
- **Manipulation des Données** : NumPy, Pandas  
- **Traitement des Images** : OpenCV, Pillow  

---

## 🚀 Pipeline de Travail  

### **Phase 1 : Classification d'Images**  
- **Objectif** : Classifier les images en catégories telles que photographies, croquis et schémas.  
- **Architecture du Modèle** : Vision Transformer (ViT)  
- **Étapes** :  
  1. Division des images en patches  
  2. Passage des patches par un encodeur Transformer  
  3. Classification finale via une couche softmax  
- **Dataset** : PHOTOCL (41 400 images réparties en 5 catégories)  
- **Métriques** : Accuracy, F1-score, matrice de confusion  

### **Phase 2 : Génération de Légendes**  
- **Objectif** : Générer des descriptions textuelles pertinentes à partir d'images  
- **Architecture du Modèle** : Encodeur-Décodeur Transformer  
  - **Encodeur** : Vision Transformer (ViT) pour extraire les caractéristiques visuelles  
  - **Décodeur** : Modèle Transformer personnalisé avec mécanismes d'attention  
- **Dataset** : MSCOCO pour l'entraînement et l'évaluation  
- **Métriques** : BLEU, CIDEr, METEOR  

### **Phase 3 : Déploiement Web**  
- **Objectif** : Fournir une interface web pour tester le système  
- **Fonctionnalités** :  
  - Téléchargement d'images  
  - Classification automatique et génération de légendes  
  - Affichage des résultats  
- **Exécution de l'Application** :  
  ```bash
  python app.py

## Démo

Voici une démonstration du projet en action :

https://github.com/user-attachments/assets/a2c27d70-b914-4b4d-9943-b08ff6d3c739


