# Analyse-financiere-sur-la-toile

L'objectif est se servir d'un "robot" qui ira chercher les données pour nous à notre place à chaque fois que l'on s'en servira et à partir de ces données récupéreés on pourra la mettre dans une base de donnée de notre choix afin de faire des graphes à notre guise.

On a choisi de prendre comme source de données [le site sur la bourse d'Apple](https://www.nasdaq.com/market-activity/stocks/aapl/historical/)

Une fois les données récupérées elle sont mises dans un dataset et ensuite exportées au [format csv](/ressources/apple_fini.csv), on a dû utiliser l'instruction `data_fini['Date'] = pd.to_datetime(data_fini['Date'], dayfirst = True)` pour avoir le bon format de date attendu par cql étant donnée que a décidé de les mettre dans une base cql. 
