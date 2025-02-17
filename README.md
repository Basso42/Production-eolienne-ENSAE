# Projet Python : Éoliennes, Vent et Production Électrique

## Introduction

L'objectif de ce projet est de prédire l'énergie produite par l'ensemble du parc éolien en France. Pour cela, nous avons croisé trois bases de données :

- Une **base de données du parc éolien français** fournissant la localisation et la longueur des pales des éoliennes en France.
- Une **base de données météorologiques** fournissant l'historique et la prévision sur 4 jours des vitesses du vent à une hauteur de 10m au-dessus du sol.
- Une **base de données de RTE** fournissant l'historique heure par heure de la production électrique éolienne nationale.

En associant les deux premières bases de données, nous pouvons approximer l'énergie produite par le parc éolien et utiliser la troisième base de données pour comparer nos résultats. Cela permet de modéliser plus fidèlement la relation entre le vent et la production électrique, et ainsi d'établir un modèle prédictif de l’énergie éolienne produite.

### 📊 Liens vers les données

- [Données du parc éolien](https://www.georisques.gouv.fr/donnees/bases-de-donnees/eolien-terrestre)
- [Données météorologiques historiques (API)](https://open-meteo.com/en/docs/historical-weather-api)
- [Données météorologiques prédites (API)](https://open-meteo.com/en/docs)
- [Données RTE (API)](https://data.rte-france.com/)

## Organisation du Notebook

L'objectif du projet était de créer un **notebook autonome**, capable de reproduire l’ensemble des résultats de manière réplicable.

Le travail est structuré en **deux grandes parties** :
1. **Récupération, nettoyage et exploration des données**.
2. **Modélisation de la relation entre le vent et la production électrique**.

### 📂 Fichiers principaux :
- **`Eoliennes_VF.ipynb`** : Notebook principal conçu pour être **parfaitement reproductible** sur le SSP Cloud de l'INSEE.
- **`Donnees_vent.ipynb`** : Notebook permettant de récupérer manuellement les données téléchargées depuis le SSP Cloud.

---

Ce projet constitue une première approche pour améliorer la prévision de la production éolienne en France en exploitant les données disponibles. 
