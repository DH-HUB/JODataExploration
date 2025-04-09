# Analyse Exploratoire des JO d'Hiver

Ce projet vise à explorer et interpréter les données des Jeux Olympiques d'hiver à travers une approche professionnelle mêlant visualisation, analyse descriptive et storytelling stratégique.

---

## Objectifs du projet

- Analyser les caractéristiques clés des athlètes (âge, taille, sexe…)
- Identifier des insights exploitables par des décideurs (fédération, analystes sportifs)
- Mettre en œuvre une approche de **Data Storytelling** directement intégrée dans les visualisations
- Préparer le jeu de données à une future modélisation (machine learning ou prédiction)

---

## Fichiers inclus

| Fichier | Description |
|--------|-------------|
| `JO_Data_Exploration.ipynb` | Notebook principal avec analyses, visualisations et storytelling intégré |
| `README.md` | Ce fichier de documentation |
| `athlete-eventscsv.zip` *(optionnel)* | Archive des données issues de Kaggle (si pas téléchargées via API) |
a
---

## Thématiques abordées

- Répartition de l'âge par médaille et sexe
- Morphologie (taille) selon les sports
- Évolution de l'âge dans le temps
- Comparaison des performances par pays (2012 vs 2016)

---
## Aperçu visuel du projet

Voici quelques visualisations extraites du notebook :

## Répartition des données après nettoyage

Les histogrammes ci-dessous montrent que les distributions de l’âge, la taille et le poids ont été vérifiées après traitement. 
Ces visualisations permettent de confirmer la qualité et la normalité des données utilisées.
![image](https://github.com/user-attachments/assets/d7f0625b-7fce-47d9-98b6-578702319de4)

### Répartition de l’âge par médaille et sexe
![image](https://github.com/user-attachments/assets/3fc2eff3-1d0a-4bd3-9898-96a7c77ff797)

### Taille des athlètes selon le sport
![image](https://github.com/user-attachments/assets/591dd2a6-b6fb-4671-8d14-4aaa34d38323)

### Évolution de l’âge dans le temps (par sexe)
![image](https://github.com/user-attachments/assets/84676ac8-78bc-425d-a608-a97c5d809b71)

### Barres empilées : performances par pays (2012 vs 2016)
![image](https://github.com/user-attachments/assets/ecb85ab0-5319-4583-9018-cdedf1baa6f5)

---
## Exécution du projet dans Google Colab

1. Ouvre `JO_Data_Exploration.ipynb` dans [Google Colaboratory](https://colab.research.google.com/)

### Deux options pour importer les données :

---

### Option A : Fichier CSV local fourni
- Décompresser le fichier `athlete-eventscsv.zip` manuellement
- Charger le fichier `.csv` dans Colab avec :

```python
import pandas as pd
df = pd.read_csv("athlete_events.csv")
```

---

### Option B : Connexion via jeton Kaggle *(intégré dans le notebook)*

- Le code complet permettant d’utiliser l’API Kaggle est **déjà inclus** dans le notebook.
- Il vous suffit de :
  1. Générer votre `kaggle.json` depuis [kaggle.com/account](https://www.kaggle.com/account)
  2. L’uploader dans l’environnement Colab
  3. Exécuter les cellules prévues (étapes de configuration + téléchargement automatique)

> Aucun besoin de modifier manuellement, tout est prêt dans le notebook.

---

## Exemple de storytelling intégré

> “Les femmes décrochent leurs médailles en moyenne plus jeunes que les hommes, ce qui peut indiquer un pic de performance plus précoce. Cette variable croisée (âge × sexe) pourrait être intégrée dans un modèle de prédiction.”

---

## Auteur

Projet réalisé par **Hakima Djermouni**  
Dataset : Kaggle - Athlete Events  
Notebook exécuté et testé sous Google Colaboratory



