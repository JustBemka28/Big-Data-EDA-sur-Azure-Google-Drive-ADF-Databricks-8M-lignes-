# Traitement de données criminelles avec Azure & Spark (8M lignes)

Ce projet illustre la mise en place d’un mini-pipeline cloud pour l’analyse exploratoire d’un jeu de données de grande taille (8 millions de lignes) en utilisant les services Azure.

## 📊 Objectif
Explorer et nettoyer un jeu de données criminelles pour en faciliter l’analyse, la compréhension et la visualisation.

## 🧰 Outils utilisés

- **Azure Data Factory** : pour l’ingestion de données depuis Google Drive
- **Azure Storage Account** : pour le stockage des fichiers bruts
- **Azure Databricks (Spark + Python)** : pour le traitement, l’EDA et la visualisation
- **PySpark** : pour la transformation, le nettoyage, la manipulation
- **Seaborn / Matplotlib** : pour les graphiques

## 🔄 Pipeline

1. 📥 **Ingestion** : via un pipeline Azure Data Factory (source HTTP → Azure Blob)
2. 🚀 **Traitement Spark** :
   - Chargement du CSV (8M lignes)
   - Renommage des colonnes en français
   - Conversion des dates en format timestamp
   - Suppression des valeurs nulles et doublons
   - Visualisation des types d’infractions, années, etc.

## 📁 Structure du projet

- `notebooks/` : Notebook Databricks pour l’analyse
- `pipeline/` : Fichiers liés à Azure Data Factory
- `Crimes.csv` : Exemple de fichier source (ou lien vers Google Drive)

## 🔗 Données

[Lien vers Google Drive pour télécharger le fichier]([https://drive.google.com/...](https://drive.google.com/file/d/157qJvi8bd5Gug2mBMyKzKzKZE71Us7_K/view?usp=sharing)
