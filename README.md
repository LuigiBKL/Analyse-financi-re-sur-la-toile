# Analyse-financiere-sur-la-toile

L'objectif est se servir d'un "robot" qui ira chercher les données pour nous à notre place à chaque fois que l'on s'en servira et à partir de ces données récupéreés on pourra la mettre dans une base de donnée de notre choix afin de faire des graphes à notre guise.

On a choisi de prendre comme source de données [le site sur la bourse d'Apple](https://www.nasdaq.com/market-activity/stocks/aapl/historical/)

Une fois les données récupérées elle sont mises dans un dataset et ensuite exportées au [format csv](/ressources/apple_fini.csv), on a dû utiliser l'instruction `data_fini['Date'] = pd.to_datetime(data_fini['Date'], dayfirst = True)` pour avoir le bon format de date attendu par mysql. Ce fichier csv sera ensuite insérer dans une [base.sql](/ressources/data_cours_apple.sql).


## Installation

On aura besoin du logiciel suivant:
- [Docker desktop pour windows](https://www.docker.com/products/docker-desktop) pour gérer nos diffirénts conteneurs

![image](/Capture1.png)

`##Infos supplémentaires:`
##Manipulation à faire

Ouvrir le cmd se situer dans le dossier ou l'on souhaite travailer à l'aide de la commande 
- cd de l'invite de commande
puis faire:
- `git clone https://github.com/LuigiBKL/Analyse-financi-re-sur-la-toile`
- `docker-compose up -d`
