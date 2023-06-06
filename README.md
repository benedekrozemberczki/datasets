# Datasets ![License](https://img.shields.io/github/license/benedekrozemberczki/datasets.svg?color=blue) [![repo size](https://img.shields.io/github/repo-size/benedekrozemberczki/datasets.svg)](https://github.com/benedekrozemberczki/datasets/archive/master.zip) [![benedekrozemberczki](https://img.shields.io/twitter/follow/benrozemberczki?style=social&logo=twitter)](https://twitter.com/intent/follow?screen_name=benrozemberczki)

Datasets collected for network science, graph mining, deep learning and general machine learning research.

<p align="center">
  <img width="600" src="/images/field.png">
</p>

##### Contents   

1. [Twitch Gamers](#twitch-gamers)
2. [LastFM Asia Social Network](#lastfm-asia-social-network)
3. [Deezer Europe Social Network](#deezer-europe-social-network)
4. [GitHub StarGazer Graphs](#github-stargazer-graphs)
5. [Twitch Ego Nets](#twitch-ego-nets)
6. [Reddit Thread Graphs](#reddit-thread-graphs)  
7. [Deezer Ego Nets](#deezer-ego-nets)
8. [GitHub Social Network](#github-social-network)
9. [Deezer Social Networks](#deezer-social-networks)
10. [Facebook Page-Page Networks](#facebook-page-page-networks)  
11. [Wikipedia Article Networks](#wikipedia-article-networks)
12. [Twitch Social Networks](#twitch-social-networks)
13. [Facebook Large Page-Page Network](#facebook-large-page-page-network)

## Twitch Gamers
<p align="center">
  <img width="200" src="/images/twitch.png">
</p>


### Description
<p align="justify">
A social network of Twitch users collected from the public API in Spring 2018. Nodes are Twitch users and edges are mutual follower relationships between them. The graph forms a single strongly connected component without missing attributes. The machine learning tasks related to the graph are count data regression and node classification. There are 6 specific tasks:</p>

- Explicit content streamer identification.
- Broadcaster language prediction.
- User lifetime estimation.
- Churn prediction.
- Affiliate status identification.
- View count estimation.

### Links


- [Twitch Gamers](https://graphai-datasets.web.app/twitch_gamers.zip)

### Properties

- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Node labels:** Yes.
- **Temporal:** No.


|   | **Twitch Gamers**  |
|---|---|
| **Nodes** |168,114   |
| **Edges** | 6,797,557 |
| **Density** |  0.0005 |
| **Transitvity** | 0.0184|

### Possible tasks

- **Binary node classification**
- **Multi-class node classification**
- **Count data regression**
- **Link prediction**
- **Community detection**
- **Community detection with ground truth**
- **Network visualization**

### Citing
```bibtex
>@misc{rozemberczki2021twitch,
       title = {Twitch Gamers: a Dataset for Evaluating Proximity Preserving and Structural Role-based Node Embeddings}, 
       author = {Benedek Rozemberczki and Rik Sarkar},
       year = {2021},
       eprint = {2101.03091},
       archivePrefix = {arXiv},
       primaryClass = {cs.SI}
       }
```

## LastFM Asia Social Network

<p align="center">
  <img width="200" src="/images/lastfm.png">
</p>



### Description
<p align="justify">
A social network of LastFM users which was collected from the public API in March 2020. Nodes are LastFM users from Asian countries and edges are mutual follower relationships between them. The vertex features are extracted based on the artists liked by the users. The task related to the graph is multinomial node classification - one has to predict the location of users. This target feature was derived from the country field for each user. </p>

### Links

- [LastFM Asia Social Network](https://graphai-datasets.web.app/lasftm_asia.zip)

### Properties

- **Directed:** No.
- **Node features:** Yes.
- **Edge features:** No.
- **Node labels:** Yes. Multinomial.
- **Temporal:** No.

|   | **LastFM**  |
|---|---|
| **Nodes** |7,624  | 
| **Edges** | 27,806  |
| **Density** |  0.001 | 
| **Transitvity** | 0.179 | 

### Possible tasks

- **Multi-class node classification**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing
```bibtex
@inproceedings{feather,
               title={{Characteristic Functions on Graphs: Birds of a Feather, from Statistical Descriptors to Parametric Models}},
               author={Benedek Rozemberczki and Rik Sarkar},
               year={2020},
	       pages={1325–1334},
	       booktitle={Proceedings of the 29th ACM International Conference on Information and Knowledge Management (CIKM '20)},
	       organization={ACM},
}
```


## Deezer Europe Social Network

<p align="center">
  <img width="200" src="/images/deezer.jpg">
</p>



### Description
<p align="justify">
A social network of Deezer users which was collected from the public API in March 2020. Nodes are Deezer users from European countries and edges are mutual follower relationships between them. The vertex features are extracted based on the artists liked by the users. The task related to the graph is binary node classification - one has to predict the gender of users. This target feature was derived from the name field for each user. </p>

### Links

- [Deezer Europe Social Network](https://snap.stanford.edu/data/feather-deezer-social.html)

### Properties

- **Directed:** No.
- **Node features:** Yes.
- **Edge features:** No.
- **Node labels:** Yes. Binary.
- **Temporal:** No.

|   | **Deezer**  |
|---|---|
| **Nodes** |28,281 | 
| **Edges** | 92,752  |
| **Density** |  0.0002 | 
| **Transitvity** | 0.0959 | 

### Possible tasks

- **Binary node classification**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing
```bibtex
@inproceedings{feather,
               title={{Characteristic Functions on Graphs: Birds of a Feather, from Statistical Descriptors to Parametric Models}},
               author={Benedek Rozemberczki and Rik Sarkar},
               year={2020},
	       pages={1325–1334},
	       booktitle={Proceedings of the 29th ACM International Conference on Information and Knowledge Management (CIKM '20)},
	       organization={ACM},
}
```

## GitHub StarGazer Graphs
<p align="center">
  <img width="200" src="/images/Octocat.png">
</p>

### Description
<p align="justify">
The social networks of developers who starred popular machine learning and web development repositories (with at least 10 stars) until 2019 August. Nodes are users and links are follower relationships. The task is to decide whether a social network belongs to a web or machine learning repository. We only included the largest component (at least with 10 users) of graphs.</p>

### Link

- [GitHub StarGazer Graphs + Target](https://graphai-datasets.web.app/graph_classification/git_stargazers.zip)

### Properties

- **Number of graphs:** 12,725
- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Graph labels:** Yes. Binary-labeled.
- **Temporal:** No.

|   | **Min**  |**Max**  |
|---|---|---|
| **Nodes** |10   | 957  | 
| **Density** | 0.003 |0.561   | 
| **Diameter** |  2 | 18 | 

### Possible Tasks
- **Graph classification**

### Citing

```bibtex
@inproceedings{karateclub,
       title = {{Karate Club: An API Oriented Open-source Python Framework for Unsupervised Learning on Graphs}},
       author = {Benedek Rozemberczki and Oliver Kiss and Rik Sarkar},
       year = {2020},
       pages = {3125–3132},
       booktitle = {Proceedings of the 29th ACM International Conference on Information and Knowledge Management (CIKM '20)},
       organization = {ACM},
}
```

## Twitch Ego Nets
<p align="center">
  <img width="200" src="/images/twitch.png">
</p>

### Description
<p align="justify">
The ego-nets of Twitch users who participated in the partnership program in April 2018. Nodes are users and links are friendships. The binary classification task is to predict using the ego-net whether the ego user plays a single or multple games. Players who play a single game usually have a more dense ego-net.</p>

### Link

- [Twitch Ego Nets Part I](https://graphai-datasets.web.app/graph_classification/twitch_egos_1.zip)
- [Twitch Ego Nets Part II + Target](https://graphai-datasets.web.app/graph_classification/twitch_egos_2.zip)

### Properties

- **Number of graphs:** 127,094
- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Graph labels:** Yes. Binary-labeled.
- **Temporal:** No.

|   | **Min**  |**Max**  |
|---|---|---|
| **Nodes** |14   | 52  | 
| **Density** | 0.038 |0.967   | 
| **Diameter** |  1 | 2 | 

### Possible Tasks
- **Graph classification**

### Citing

```bibtex
@inproceedings{karateclub,
       title = {{Karate Club: An API Oriented Open-source Python Framework for Unsupervised Learning on Graphs}},
       author = {Benedek Rozemberczki and Oliver Kiss and Rik Sarkar},
       year = {2020},
       pages = {3125–3132},
       booktitle = {Proceedings of the 29th ACM International Conference on Information and Knowledge Management (CIKM '20)},
       organization = {ACM},
}
```

## Reddit Thread Graphs

<p align="center">
  <img width="200" src="/images/reddit-logo-png-transparent.png">
</p>

### Description
<p align="justify">
Discussion and non-discussion based threads from Reddit which we collected in May 2018. Nodes are Reddit users who participate in a discussion and links are replies between them. The task is to predict whether a thread is discussion based or not (binary classification). </p>

### Link

- [Reddit Thread Graphs + Target](https://graphai-datasets.web.app/datasets/graph_classification/reddit_threads.zip)

### Properties

- **Number of graphs:** 203,088
- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Graph labels:** Yes. Binary-labeled.
- **Temporal:** No.

|   | **Min**  |**Max**  |
|---|---|---|
| **Nodes** |11   | 97  | 
| **Density** | 0.021 |0.382   | 
| **Diameter** |  2 | 27 | 

### Possible Tasks
- **Graph classification**

### Citing

```bibtex
@inproceedings{karateclub,
       title = {{Karate Club: An API Oriented Open-source Python Framework for Unsupervised Learning on Graphs}},
       author = {Benedek Rozemberczki and Oliver Kiss and Rik Sarkar},
       year = {2020},
       pages = {3125–3132},
       booktitle = {Proceedings of the 29th ACM International Conference on Information and Knowledge Management (CIKM '20)},
       organization = {ACM},
}
```

## Deezer Ego Nets

<p align="center">
  <img width="200" src="/images/deezer.jpg">
</p>

### Description
<p align="justify">
The ego-nets of Eastern European users collected from the music streaming service Deezer in February 2020. Nodes are users and edges are mutual follower relationships. The related task is the prediction of gender for the ego node in the graph.</p>

### Link

- [Deezer Ego Nets + Target](https://graphai-datasets.web.app/graph_classification/deezer_egos.zip)

### Properties

- **Number of graphs:** 9,629
- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Graph labels:** Yes. Binary-labeled.
- **Temporal:** No.

|   | **Min**  |**Max**  |
|---|---|---|
| **Nodes** |11   | 363  | 
| **Density** | 0.015 |0.909   | 
| **Diameter** |  2 | 2 | 

### Possible Tasks
- **Graph classification**

### Citing

```bibtex
@inproceedings{karateclub,
       title = {{Karate Club: An API Oriented Open-source Python Framework for Unsupervised Learning on Graphs}},
       author = {Benedek Rozemberczki and Oliver Kiss and Rik Sarkar},
       year = {2020},
       pages = {3125–3132},
       booktitle = {Proceedings of the 29th ACM International Conference on Information and Knowledge Management (CIKM '20)},
       organization = {ACM},
}
```


## GitHub Social Network
<p align="center">
  <img width="200" src="/images/Octocat.png">
</p>

### Description
<p align="justify">
A large social network of GitHub developers which was collected from the public API in June 2019. Nodes are developers who have starred at least 10 repositories and edges are mutual follower relationships between them. The vertex features are extracted based on the location, repositories starred, employer and e-mail address. The task related to the graph is binary node classification - one has to predict whether the GitHub user is a web or a machine learning developer. This target feature was derived from the job title of each user.</p>

### Link

- [GitHub Web-ML](https://snap.stanford.edu/data/github-social.html)

### Properties

- **Directed:** No.
- **Node features:** Yes.
- **Edge features:** No.
- **Node labels:** Yes. Binary-labeled.
- **Temporal:** No.

|   | **GitHub**  |
|---|---|
| **Nodes** |37,700   | 
| **Edges** | 289,003  |
| **Density** |  0.001 | 
| **Transitvity** | 0.013| 

### Possible Tasks
- **Binary node classification**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing

```bibtex
>@article{musae,
          author = {Rozemberczki, Benedek and Allen, Carl and Sarkar, Rik},
          title = {{Multi-Scale Attributed Node Embedding}},
          journal = {Journal of Complex Networks},
          volume = {9},
          number = {2},
          year = {2021},
}
```
## Deezer Social Networks
<p align="center">
  <img width="200" src="/images/deezer.jpg">
</p>

### Description
<p align="justify">
The data was collected from the music streaming service Deezer (November 2017). These datasets represent friendship networks of users from 3 European countries. Nodes represent the users and edges are the mutual friendships. We reindexed the nodes in order to achieve a certain level of anonimity. The csv files contain the edges - nodes are indexed from 0. The json files contain the genre preferences of users - each key is a user id, the genres loved are given as lists. Genre notations are consistent across users. In each dataset users could like 84 distinct genres. Liked genre lists were compiled based on the liked song lists. The countries included are Romania, Croatia and Hungary. For each dataset we listed the number of nodes an edges.</p>

### Links

- [Romania](http://snap.stanford.edu/data/gemsec-Deezer.html)
- [Croatia](http://snap.stanford.edu/data/gemsec-Deezer.html)
- [Hungary](http://snap.stanford.edu/data/gemsec-Deezer.html)

### Properties

- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Node labels:** Yes. Multi-labeled.
- **Temporal:** No.

|   | **RO**  | **HR**  | **HU**  |
|---|---|---|---|
| **Nodes** |41,773   | 54,573  |  47,538 |
| **Edges** | 125,826  |498,202 |  222,887 |
| **Density** |  0.0001 | 0.0004  | 0.0002 |
| **Transitvity** | 0.0752| 0.1146 | 0.0929 |

### Possible Tasks

- **Node classification**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing

If you find these datasets useful in your research, please cite the following paper:

```bibtex
>@inproceedings{rozemberczki2019gemsec,    
                title={GEMSEC: Graph Embedding with Self Clustering},    
                author={Rozemberczki, Benedek and Davies, Ryan and Sarkar, Rik and Sutton, Charles},    
                booktitle={Proceedings of the 2019 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining 2019},    
                pages={65-72},    
                year={2019},    
                organization={ACM}    
                }
```
## Facebook Page-Page Networks
<p align="center">
  <img width="200" src="/images/facebook.png">
</p>

### Description
<p align="justify">
We collected data about Facebook pages (November 2017). These datasets represent blue verified Facebook page networks of different categories. Nodes represent the pages and edges are mutual likes among them. The csv files contain the edges - nodes are indexed from 0. We included 8 different distinct types of pages. These are listed below. For each dataset we listed the number of nodes an edges.
</p>

### Links

- [Politicians](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [Companies](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [Athletes](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [Media](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [Public Figures](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [Artists](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [Government](http://snap.stanford.edu/data/gemsec-Facebook.html)
- [TV Shows](http://snap.stanford.edu/data/gemsec-Facebook.html)

### Properties

- **Directed:** No.
- **Node features:** No.
- **Edge features:** No.
- **Node labels:** No.
- **Temporal:** No.

|   | **Nodes**  | **Edges**  | **Density**  | **Transitvity**|
|---|---|---|---|---|
| **Politicians**|  	5,908| 	41,729|0.0024|0.3011|
| **Companies**| 	14,113| 	52,310|0.0005|0.1532|
| **Athletes**| 		13,866| 	86,858|0.0009|0.1292|
| **News Sites**| 		27,917| 	206,259|0.0005|0.1140|
| **Public Figures**| 		11,565| 	67,114|0.0010|0.1666|
| **Artists**|  	50,515| 	819,306|0.0006|0.1140|
| **Government**| 		7,057|		89,455|0.0036|0.2238|
| **TV Shows**| 		3,892| 	17,262|0.0023|0.5906|

### Possible Tasks

- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing

If you find these datasets useful in your research, please cite the following paper:

```bibtex
>@inproceedings{rozemberczki2019gemsec,    
                title={GEMSEC: Graph Embedding with Self Clustering},    
                author={Rozemberczki, Benedek and Davies, Ryan and Sarkar, Rik and Sutton, Charles},    
                booktitle={Proceedings of the 2019 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining 2019},    
                pages={65-72},    
                year={2019},    
                organization={ACM}    
                }
```
       
## Wikipedia Article Networks
<p align="center">
  <img width="400" src="/images/wikipedia-logo.jpg">
</p>

### Description
<p align="justify">
The data was collected from the English Wikipedia (December 2018). These datasets represent page-page networks on specific topics (chameleons, crocodiles and squirrels). Nodes represent articles and edges are mutual links between them. The edges csv files contain the edges - nodes are indexed from 0. The features json files contain the features of articles - each key is a page id, and node features are given as lists. The presence of a feature in the feature list means that an informative noun appeared in the text of the Wikipedia article. The target csv contains the node identifiers and the average monthly traffic between October 2017 and November 2018 for each page.  For each page-page network we listed the number of nodes an edges with some other descriptive statistics.
</p>

### Links

- [Wikipedia Chameleons](http://snap.stanford.edu/data/wikipedia-article-networks.html)
- [Wikipedia Crocodiles](http://snap.stanford.edu/data/wikipedia-article-networks.html)
- [Wikipedia Squirrels](http://snap.stanford.edu/data/wikipedia-article-networks.html)

### Properties

- **Directed:** No.
- **Node features:** Yes.
- **Edge features:** No.
- **Node labels:** Yes. Continuous target.
- **Temporal:** No.

|   | **Chameleon**  | **Crocodile**  | **Squirrel**  |
|---|---|---|---|
| **Nodes** |2,277   | 11,631  |  5,201 |
| **Edges** | 31,421  |170,918 |  198,493 |
| **Density** |  0.012 | 0.003  | 0.015 |
| **Transitvity** | 0.314| 0.026 | 0.348 |

### Possible Tasks

- **Regression**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing

If you find these datasets useful in your research, please cite the following paper:

```bibtex
>@article{musae,
          author = {Rozemberczki, Benedek and Allen, Carl and Sarkar, Rik},
          title = {{Multi-Scale Attributed Node Embedding}},
          journal = {Journal of Complex Networks},
          volume = {9},
          number = {2},
          year = {2021},
}
```
## Twitch Social Networks
<p align="center">
  <img width="200" src="/images/twitch.png">
</p>


### Description
<p align="justify">
These datasets used for node classification and transfer learning are Twitch user-user networks of gamers who stream in a certain language. Nodes are the users themselves and the links are mutual friendships between them. Vertex features are extracted based on the games played and liked, location and streaming habits. Datasets share the same set of node features, this makes transfer learning across networks possible. These social networks were collected in May 2018. The supervised task related to these networks is binary node classification - one has to predict whether a streamer uses explicit language.</p>

### Links


- [Germany](http://snap.stanford.edu/data/twitch_gamers.html)
- [England](http://snap.stanford.edu/data/twitch_gamers.html)
- [Spain](http://snap.stanford.edu/data/twitch_gamers.html)
- [France](http://snap.stanford.edu/data/twitch_gamers.html)
- [Porutgal](http://snap.stanford.edu/data/twitch_gamers.html)
- [Russia](http://snap.stanford.edu/data/twitch_gamers.html)
- [Taiwan](http://snap.stanford.edu/data/twitch_gamers.html)

### Properties

- **Directed:** No.
- **Node features:** Yes.
- **Edge features:** No.
- **Node labels:** Yes. Binary-labeled.
- **Temporal:** No.


|   | **DE**  | **EN**  | **ES**  |**FR**  | **PT**  | **RU**  |**TW**  |
|---|---|---|---|---|---|---|---|
| **Nodes** |9,498   | 7,126  |  4,648 |6,549   | 1,912  |  4,385 |2,772 |
| **Edges** | 153,138  |35,324 |  59,382 |112,666   | 31,299  |  37,304 |63,462 |
| **Density** |  0.003 | 0.002  | 0.006 | 0.005   | 0.017  |  0.004 |0.017|
| **Transitvity** | 0.047| 0.042 | 0.084 |0.054   | 0.131  |  0.049 |0.120 |

### Possible tasks

- **Binary node classification**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing
```bibtex
>@article{musae,
          author = {Rozemberczki, Benedek and Allen, Carl and Sarkar, Rik},
          title = {{Multi-Scale Attributed Node Embedding}},
          journal = {Journal of Complex Networks},
          volume = {9},
          number = {2},
          year = {2021},
}
```
## Facebook Large Page-Page Network
<p align="center">
  <img width="200" src="/images/facebook.png">
</p>



### Description
<p align="justify">
This webgraph is a page-page graph of verified Facebook sites. Nodes represent official Facebook pages while the links are mutual likes between sites. Node features are extracted from the site descriptions that the page owners created to summarize the purpose of the site. This graph was collected through the Facebook Graph API in November 2017 and restricted to pages from 4 categories which are defined by Facebook. These categories are: politicians, governmental organizations, television shows and companies. The task related to this dataset is multi-class node classification for the 4 site categories. </p>

### Links

- [Facebook Large Page-Page](http://snap.stanford.edu/data/facebook-large-page-page-network.html)

### Properties

- **Directed:** No.
- **Node features:** Yes.
- **Edge features:** No.
- **Node labels:** Yes. Multinomial.
- **Temporal:** No.

|   | **Facebook**  |
|---|---|
| **Nodes** |22,470   | 
| **Edges** | 171,002  |
| **Density** |  0.001 | 
| **Transitvity** | 0.232| 

### Possible tasks

- **Multi-class node classification**
- **Link prediction**
- **Community detection**
- **Network visualization**

### Citing
```bibtex
>@article{musae,
          author = {Rozemberczki, Benedek and Allen, Carl and Sarkar, Rik},
          title = {{Multi-Scale Attributed Node Embedding}},
          journal = {Journal of Complex Networks},
          volume = {9},
          number = {2},
          year = {2021},
}
```
--------
