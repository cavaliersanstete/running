# README

Ce projet a pour but d'exploiter les données de mes courses à pied afin de prédire ma forme. 

### Problème rencontrer pour la connexcion à l'api de garmin connect. 

Derrière garmin login c'est garth qui est utilisé avec la méthode garth loggin, et garth.connectapi.
Le problème original est la politique de garmin de sécurité des données. L'API est réservé aux entreprises, par exemples runanalyze. 
Si j'ai bien compris les explications reddit https://www.reddit.com/r/Garmin/comments/114eh9y/personal_use_of_garmin_api/?rdt=53755 , 
pour contourner les problèmes l'api de cyber-junky sur github est utilisé garth pour se faire passer pour le navigateur. 
Une autre solution pour récupérer les données est d'utiliser GarminDB.

https://news.ycombinator.com/item?id=42912515 autres discussions intéressantes sur le sujet. 

Le nombre de requete autorisé à l'API est 2 par jours, apparement. 