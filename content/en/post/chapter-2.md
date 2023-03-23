---
date: 2023-02-10T11:00:59-04:00
description: "Implémentation d'un modèle de scoring et déploiement sur AWS"
featured_image: "/images/scoring.jpg"
tags: ["scene"]
title: "Projet 2: Scoring des clients d'une société financière"
---

- [x] Amazon Web Services  - [x] Smote - [x] Docker - [x] Github CI/CD - [x] GridSearchCV - [x] Streamlit - [x] Flask - [x] SHAP

Dans ce projet j'ai mis en place un outils de **scoring crédit** pour calculer la probabilité qu'un client rembourse son crédit, et classifier la demande en **accordé** ou **refusé**.
Pour réaliser cette tache, j'ai mis en place un algorithme de classification s'appuyant sur des sources de données variées. Puis j'ai créé un dashboard interactif, permettant de prédire les scores des clients, que j'ai déployé sur le cloud d'**Amazon Web Services**.
Les principaux challenges de ce projet étaient la grande quantité de features qui nécessitaient un feature engineering pointu, la gestion du déséquilibre des classes et l'implémentation d'une **fonction coût métier** adapté à notre problématique.
Etapes:
* Analyse exploratoire et **feature engineering** ayant permis de gérer les valeurs extremes et les valeurs manquantes.
* Mise en place de pipelines de modélisation et test de trois modèle différents: **Régression logistique**, **Forêts aléatoires** et **LightGBM** avec tuning des **hyperparamètres** et **Cross Validation** par **GridSearchCV**.
* Scoring à travers une **fonction coût métier** que j'ai implémenté.
* La gestion du déséquilibre des classes a été faite avec la librairie **Smote** et implémenter directement à l'intérieur des pipelines pour éviter une fuite de données.
* Implémentation d'un modèle SHAP pour l'explicabilité du modèle de scoring.
{{< figure src="/images/shap.png" >}}

* Création d'un dashboard interactif à l'aide de **Streamlit**
* Création d'une **API REST** sous **Flask** pour la gestion du modèle dans le cloud
* Déploiement du dashboard sur **Amazon Elastic Beanstalk** via un conteneur **Docker** et un déploiement contenu **Github CI/CD**
{{< figure src="/images/dashboard.png" >}}

[Répertoire Github du projet](https://github.com/azioba/projet_7_deployment)