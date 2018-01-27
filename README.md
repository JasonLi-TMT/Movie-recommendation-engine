# Film recommendation engine based on Google Cloud

## Data description:

In this project, I mainly use two datasets, one is film rating data, and the other is movie poster data. 

+ Film rating data: Consist of 100,005 film rating records. (link: http://www.grouplens.org/node/73)

+ Film poster data: Movie poster data from IMDB & TMDB. (link: https://www.themoviedb.org/?language=en)


The detail of data description could be found in the data folder, there is a readme file there.

## Environment: 

1: Python environment setting is in the doc folder called environment.

2: Google Cloud: Including linux environment and GPU (Telsa K80). EC2 Url: https://35.227.55.209:5000 currently stopped due to cost, plz contact zl2528@columbia.edu to get access.

## Target:

1: Classify the data into ten labels.

2: Predict the next 25 sequence data with dirty data.

## Model:

1: Classification: GRU, LSTM, SimpleRNN, the model I trained is in the code-model folder saved as keras model. For GRU and Simple RNN, it achieve 93%, 91% accuracy rate, and for LSTM, it gets 83% accuracy rate

2: Predictions: GRU, LSTM, I classify the data into quantiles and use accuracy rate as target, but the result is not quite good, only 63% accuracy rate achieved due to time, compuational power & knowledge limitaion.

## some screenshot
