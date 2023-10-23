### Projet Python : Eoliennes, vent et production électrique
#### Introduction

L'objectif de ce projet est de prédire l'énergie produite par l'ensemble du parc éolien en France. Pour cela, nous avons couplé trois bases de données :

- Une base de données du parc éolien français fournissant la localisation et la longueur des pales des éoliennes sur le territoire français
- Une base de données météorologiques fournissant l'historique et la prévision sur 4 jours des vitesses du vent a une hauteur de 10m audessus du sol
- Une base de données de RTE fournissant l'historique heure par heure de la production électrique éolienne nationale

En associant les deux premières bases de données, nous pouvons approximer l'énergie produite par le parc éolien et utiliser la troisième base de données pour comparer nos résultats et modéliser plus fidèlement la relation entre vent et production électrique et ainsi trouver une relation pour prédire l'énergie éolienne produite.
Liens vers les données

- [Données du parc éolien](https://www.georisques.gouv.fr/donnees/bases-de-donnees/eolien-terrestre)
- [Données météorologiques historiques via API](https://open-meteo.com/en/docs/historical-weather-api)
- [Données météorologiques prédites via API](https://open-meteo.com/en/docs)
- [Données RTE via API](https://data.rte-france.com/)

#### Organisation du notebook

Le but de cet exercice était de d'avoir un notebook autonome, permettant de récupérer l'ensemble des résultats. 

Une première partie composée de la récupération, du nettoyage et de l'exploration des données suivie d'une seconde portant sur la modélisation.

Le notebook principal Eoliennes_VF a été conçu pour être parfaitement reproductible depuis le SSP Cloud de l'INSEE.
Le notebook Donnees_vent permet de récupérer manuellement les données téléchargées depuis le SSP Cloud.
