# Projet : Exploration et Analyse de Données Amazon - Sports and Outdoors

Ce projet à pour objectif de traiter et analyser un jeu de données issu de la plateforme Amazon, en se focalisant sur la catégorie **Sports and Outdoors**. Réalisé en groupe de 3 étudiants, il se divise en plusieurs parties qui explorent des motifs fréquents, l'extraction de motifs à forte utilité, et la découverte de groupes d'utilisateurs partageant des habitudes d'achats similaires.

## 📂 Architecture du projet
```
. ├── data
  │   ├── dataClean.ipynb # Script de pré-traitement des données 
  │   └── df.csv # Jeu de données nettoyé 
  ├── doc
  │   └── EDA_Cardi_Ferroni_Moyo-Kamdem.pdf
  ├── README.md # Documentation du projet 
  └── src 
      ├── Partie1.ipynb # Analyse des motifs fréquents 
      ├── Partie2.ipynb # Extraction des motifs à forte utilité 
      └── Partie3.ipynb # Découverte et évaluation des groupes d'utilisateurs
```

---

## 🎯 Objectifs

### Partie 1 : Analyse des motifs fréquents
- Identifier les motifs fréquents dans les données.
- Étudier l'apport des motifs fermés.
- Extraire les règles d'association les plus confiantes.
- Identifier des comportements spécifiques à des sous-populations.
- Proposer une collection de motifs qui comprime efficacement les données.

### Partie 2 : Extraction des motifs à forte utilité
- Découvrir des motifs fréquents selon des contraintes spécifiques.
- Prendre en compte les **utilités des items** à l'aide de l'algorithme générique **QPlus**.
- Proposer un système d'extraction de motifs à la demande et justifier le choix de l'approche.
- Effectuer une étude qualitative sur un échantillon d'au moins **1000 motifs**.

### Partie 3 : Découverte de groupes d'utilisateurs
- Proposer une définition de groupe en fonction des attributs disponibles (ex. : fréquence d'achat, notes, prix moyen).
- Évaluer les groupes en termes de **couverture**, **diversité**, **distribution des notes** et **fréquence d'achat**.
- Adapter l'algorithme **MOMRI** au jeu de données.
- Effectuer une synthèse sur le **temps d'exécution**, la **qualité des groupes obtenus**, et les **insights** obtenus.

---

## 📊 Jeu de données
Le jeu de données utilisé est extrait du dataset **[Amazon Review Dataset](https://cseweb.ucsd.edu/~jmcauley/datasets/amazon_v2/)**, publié par Jianmo Ni, Jiacheng Li et Julian McAuley dans leur article : 
> **Jianmo Ni, Jiacheng Li, Julian McAuley**  
> Empirical Methods in Natural Language Processing (EMNLP), 2019

### Description
- **Catégorie analysée** : Sports and Outdoors
- **Attributs principaux** :
  - `rating` : Note attribuée par les utilisateurs.
  - `user` : Identifiant de l'utilisateur.
  - `item` : Identifiant de l'article.
  - `price` : Prix de l'article.

---

## ✨ Résultats
- Les résultats obtenus pour chaque partie sont disponibles dans les notebooks correspondants :
  - Partie 1 : **Identification des motifs fréquents** et **règles d'association**.
  - Partie 2 : **Extraction de motifs à forte utilité** avec **QPlus**.
  - Partie 3 : **Groupes d'utilisateurs** optimisés selon les métriques de couverture, diversité et diamètre (via **α-MOMRI** et **h-MOMRI**).
