# deep-learning-classification-chiens
Classification d'images de races de chiens à l'aide de réseaux de neurones convolutifs (CNN), explorant le Transfer Learning et le Fine-tuning.
# Projet Deep Learning : Classification d’images de chiens
**Auteur :** Oumayma Mourabit

### Introduction
L'objectif de ce projet est de développer un modèle de classification d'images capable de différencier cinq races de chiens en utilisant des réseaux de neurones convolutionnels (CNN). Nous avons suivi une méthodologie rigoureuse incluant l'entraînement d'un CNN from scratch, l'utilisation du Transfer Learning et l'application du fine-tuning pour améliorer les performances du modèle.

### Méthodologie

Ce projet explore différentes stratégies d'entraînement et d'optimisation afin d'obtenir un modèle performant et généralisable. La démarche suivie inclut les étapes suivantes:

1.  **Préparation des données**: Séparation des données en ensembles d'apprentissage et de test, et comparaison des performances avec et sans **augmentation de données**.
2.  **Entraînement d'un CNN from scratch**: Construction et évaluation d'un réseau CNN de base pour une approche initiale.
3.  **Transfer Learning**: Utilisation d'un modèle pré-entraîné (VGG16) pour extraire des caractéristiques, adapté à notre tâche spécifique.
4.  **Fine-tuning**: Déblocage et réentraînement des dernières couches du modèle VGG16 pour affiner les performances et les adapter au mieux aux données.
5.  **Évaluation et visualisation**: Analyse des courbes d'apprentissage, des métriques de classification et de la matrice de confusion pour évaluer et comparer les performances des différents modèles.

### Réalisations et Résultats

* **Modèle CNN from scratch:** A montré un sur-apprentissage sévère, bien que l'augmentation de données ait permis une légère amélioration de la généralisation.
* **Modèle Transfer Learning (VGG16):** A significativement amélioré les performances par rapport au modèle from scratch, atteignant une précision de validation de 53.65%.
* **Modèle Fine-tuné (VGG16):** A permis d'obtenir la meilleure performance finale, avec une **précision de 72.53%** sur l'ensemble de test.

### Pistes d'amélioration

L'analyse de la matrice de confusion a révélé des difficultés à distinguer certaines races. Des pistes d'amélioration pourraient inclure :
* L'utilisation d'architectures de modèles pré-entraînés plus récentes.
* L'optimisation des hyperparamètres.
* La collecte de données d'entraînement supplémentaires pour les classes sous-représentées.

### Environnement Technique
* **Langage :** Python
* **Librairies :** TensorFlow, Keras, Scikit-learn, NumPy, Matplotlib, Seaborn
* **Notebook :** Jupyter Notebook (pour le code et l'analyse)

### Structure du projet
.
├── notebooks/
│   └── Projet_Deep_Learning_Classification_chiens.ipynb
├── data/
│   └── (les images de chiens)
├── README.md
└── mon_modele.h5
