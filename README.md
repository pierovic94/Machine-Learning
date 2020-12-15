# Machine-Learning

## Expedia Dataset 
Welcome! This dataset was provided by the Expedia, an online travel agency (OTA) website: with logs of customer behavior. These include what customers searched for, how they interacted with search results (click/book), whether or not the search result was a travel package. The data in this dataset is a random selection from Expedia and is not representative of the overall statistics.

## Context

Expedia Group is the world's travel platform, with an extensive brand portfolio that includes some of the world's most trusted online travel brands since 1996.

Expedia has in-house algorithms to form hotel clusters, where similar hotels for a search (based on historical price, customer star ratings, geographical locations relative to city center, etc) are grouped together. These hotel clusters serve as good identifiers to which types of hotels people are going to book, while avoiding outliers such as new hotels that don't have historical data.
The datasets are split based on time: one from 2013 and 2014, while the other are from 2015. 2013-2014 data includes all the users in the logs, including both click events and booking events. 2015 data only includes booking events. 
destinations.csv data consists of features extracted from hotel reviews text. 
Note that some srch_destination_id's in the dataset files don't exist in the destinations.csv file. This is because some hotels are new and don't have enough features in the latent space. You should be able to handle this missing information whenever necessary.

## Objective
The success of Expedia is dependent on the number of bookings made. The better the hotel recommendations, the more likely is a user to book with Expedia. Therefore, it is of a foremost interest for Expedia to make the best possible predictions for users, finalize bookings, and consequently generate revenues. Given that there are hundreds of millions of visitors every month, and the recommendations have to be made instantaneous, 
it is not a small task but the rewards, also in terms of additional revenue, can be tremendous.

## Methodology (ML algorithm)
We decided to train four machine learning models and one benchmark model.

- Benchmark model
- Decision tree
- Neural network
- Bagging: Random Forest
- Boosting: XGBoost

We want to store the model objects as well as the grid search (tuning hyperparameters) results in a list to compare them in the end.
