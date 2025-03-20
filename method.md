Ce fichier sert de brouillon afin de déterminer les choix d'architecture de ce projet. 

# Objectifs :

- Accéder aux données par l'API garmin connect.

- Stocker les données de l'API de façon indépendante car les données ne sont conservées que sur une période limitée. Comme il s'agit de données perso. Il peut être intéressant de les gardé pour observer des évolutions sur une période longue. 

- Analyser les données stockés

- Réaliser des prédictions

- Faire une API ou un Streamlit. 

# Questions

## Quelle granularité temporelle choisir pour les données ? 

Nécessite d'explorer les différents champs. 

## Comment gérer les différents objets pour chaque champ ?
Les données de sommeil ne sont pas fourni par l'API dans les mêmes objets que les données de stress. 
Les activées bien que lié aux autres données, sont des objets également très différents. Liée à un temporalité courte mais répétitive.
Faut il utiliser un base de données relationnel ou NoSql. 
Les base de données NoSQL semble plus adapter au données. Cependant, je connais un peu mieux les bases de données relationnels et l'approche semble plus intéressantes pour du ML.

## Quelle idée de prédiction réaliser ? 

### Améliorer les prédictions de courses de garmin. 

**Avis** : **Difficile** car si je dispose uniquement de mes données il s'agira d'extrapolation, alors que garmin utilise sans doute des modèles d'interpolatin pour faire ses prédictions. L'écart entre la prédiction et les différentes courses réalisé montre que leur interpolation ne sont pas adapté à mon profil. 


### Prédiction de la charge d'entrainement pour élaborer les plans d'entrainement en fonction de mon niveau actuel déterminé à partir de mes données d'entrainements. 