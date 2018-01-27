# Film recommendation engine based on Google Cloud

### Key words: Python, Pyspark, SQL, GraphDB, Tensorflow, ALS, SVD, CNN, VGG16, Rating matrix

## Data description:

In this project, I mainly use two datasets, one is film rating data, and the other is movie poster data. 

- **Film rating data**: Consist of 100,005 film rating records. (link: http://www.grouplens.org/node/73)

- **Film poster data**: Movie poster data from IMDB & TMDB. (link: https://www.themoviedb.org/?language=en)

- **Film relationship data**: Data of relationship among films, directors & actors. 


The detail of data description could be found in the data folder, there is a readme file there.

## Environment & Database: 

- **Google Cloud Linux environment setting**:  

1: Spark & Hadoop Cluster setting on Google Cloud: 1 master node with 4 worker node.

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/Screen%20Shot%202018-01-27%20at%2012.03.52%20PM.png" height="250" width="500">

2: EC2 for PySpark & python coding: EC2 Url: https://35.227.55.209:5000 currently stopped due to cost, plz contact zl2528@columbia.edu to get access.

- **Database**: 

1: **Cloud SQL**: host ='104.154.165.159', user = 'root', database name: 'Spark', password: 1111

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/Screen%20Shot%202018-01-27%20at%2012.10.30%20PM.png" height="250" width="500">

2: **Graph database**: visualization of relationship among films, directors & actors

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/graph_database.png" height="250" width="500">

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/graph_database2.png" height="250" width="500">

## Target:

1: Make film recommendation with different modes

2: Ultizie google cloud and online database to scale the project

## Model:

The models used here are mostly target at performing feature engineering, including feature engineering from movie posters with CNN, extracting latent features through Spark ALS model & SVD (matrix factorization).

1: Deep learning (CNN,VGG16): Ultilized pretrained VGG16 to extract features from movie posters

2: SVD: Singular-value decomposition is a way to perform matrix factorization, it could be used to extract latent features from rating matrix. I used SVD with Tensorflow here to improve the compuational efficience.

3: Spark ALS: Spark ALS model is a spark built-in model and are widely used in the industry for recommendation system.

## Recommendation result

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/1.png" height="400" width="900">

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/2.png" height="400" width="900">

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/3.png" height="400" width="900">

<img src="https://github.com/ZishuoLi/Film-recommendation-engine-based-on-Google-Cloud/blob/master/figs/4.png" height="900" width="900">


## some screenshot
