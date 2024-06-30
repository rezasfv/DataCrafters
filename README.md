# DataCrafters' DCSSO
### DataCrafters' group work about a Graph Database for football Open Data - University of Padua, 2023 
The overall goal of this work is to collect, clean and organize statistics about football players and clubs, in order to create a Graph Database allowing to query and analyze them.

#### Datasets
Here are the URLs of the datasets we have used:
* https://www.kaggle.com/datasets/jashsheth5/indepth-soccer-statistics-xg-xa-and-more <br>
  Our main source. The dataset contains detailed seasonal statistics for every player from top European leagues from season 14/15 to season 19/20.
* https://www.kaggle.com/datasets/davidcariboo/player-scores <br>
  From here we have used overall information about players and teams, and player appearances to help us matching between different sources. <br>
  The source of these data is Transfermarkt, and they come along TM IDs of players and clubs, which are extremely useful for matching purposes.
* https://www.kaggle.com/datasets/kriegsmaschine/soccer-players-values-and-their-statistics/  <br>
  We have used this dataset to compute split statistics about players switching team during a season. It contains detailed data from season 17/18 to season 19/20, although it's not exhaustive in terms of players.  <br>
* https://understat.com/ <br>
  All the data regarding the ladders of the leagues from season 14/15 to season 19/20 were scraped from understat. <br>

#### Organization of the repository
* __rdf:__ contains all the .ttl files obtained by serialization in the notebook.
* __loadData:__ contains the datasets, the Jupyter notebook we have used for ingesting the data and some intermediate outputs.
* __dcsso:__ contains our ontology and the ones we have imorted (FOAF, SKOS).
* __queries:__ contains textual files with some queries, divided by topic.
* __SHACL:__ contains textual files with the SHACL shapes we have used to validate our data.

#### A quick overview to our model
![alt text](https://github.com/MarcoGasparini00/DataCrafters/blob/main/dcsso_graph.jpg?raw=true)
