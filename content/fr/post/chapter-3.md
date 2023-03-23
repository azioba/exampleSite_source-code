---
date: 2023-01-23T11:13:32-04:00
description: "Segmentation"
featured_image: "/images/cluster_mr.png"
tags: []
title: "Projet 3: Segmentation des clients d'un site d'E-commerce"
---

- [x] Séries temporelles  - [x] RFM - [x] ARI - [x] PCA - [x] K-means - [x] DBScan 

- Dans ce projet, ma mission consistait à comprendre les différents types de clients d'un site d'E-commerce et de réaliser une segmentation de ces clients.
J'ai donc réalisé ce projet à travers plusieurs étapes:
* Une analyse exploratoire afin de comprendre les données pour mieux les exploiter.
* Aggrégation des clients et commandes en **RFM**
* Reduction de dimension **PCA**
* Test de plusieurs méthodes de segmentation: **DBScan**, **Clustering Hierarchique**, **K-means**
{{< figure src="/images/cluster_mr.png" >}}

* Calcul de la courbe ARI et estimation du délai de maintenance du modèle
{{< figure src="/images/ari.png" >}}

Ce projet m'a permis d'aborder et surmonter des difficultés tels que le fait que seuls **3%** des clients ont passé plus d'une commande, ce qui rendait la segmentation un peu peu plus compliqué à mettre en place.


[Répertoire Github du projet](https://github.com/azioba/Client_Segmentation)
