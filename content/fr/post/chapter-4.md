---
date: 2023-01-12T11:14:48-04:00
description: "Classification d'articles, basé sur une image et une description"
featured_image: "/images/vision.jpg"
tags: ["scene"]
title: "Projet 4: NLP & Computer Vision"
---

- [x] NLP  - [x] BERT - [x] USE - [x] CNN - [x] Transfert Learning - [x] PCA

L'objectif de ce projet est l'automatisation de l'attribution d'une catégorie aux articles mis en ligne sur une site de vente en ligne.
Pour celà j'ai mis en place un **moteur de classification** des articles en différentes catégories, avec un niveau de précision suffisant.
La classification étant basée sur une image et une description, j'ai procédé par étapes:
* **Prétraitement** des données texte ou image suivant les cas.
* Extraction de features texte: **bag-of-words**, **Tf-idf**, word/sentence embedding avec **Word2Vec**, **BERT** et **USE**
* Extraction de features image: **SIFT**, **CNN Transfert Learning** avec TensorFlow
* Réduction en 2 dimensions **TSN-E**, afin de projeter les produits sur un graphique 2D.
{{< figure src="/images/tsn-e.png" >}}
