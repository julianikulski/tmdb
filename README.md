# Movie revenue predictions with data from The Movie Database

This project leverages a dataset of 3,000 movies with 22 variables from The Movie Database to predict movie revenues. Features used for prediction include gender of cast members, movie genres, budget and production companies.

## Table of Contents
* [Installation](#Installation)
* [Project Motivation](#motivation)
* [File Description](#description)
* [Results](#Results)
* [Licensing, Authors, Acknowledgements](#licensing)

## Installation
The code requires Python versions of 3.* and general libraries available through the Anaconda package.

## Project Motivation <a name="motivation"></a>
As a dedicated movie and TV show nerd myself, I wanted to get a deeper understanding of patterns within some of the most popular movies globally. Can we identify certain metrics that will make a movie an almost guaranteed success? What role does gender or the genres play? During times of peak movie franchises, how do prequels or sequels of a movie factor into the overall success? I am going to answer these and more questions in this project but will focus on two main issues:

1. Which variables are particularly predictive of absolute revenue figures?
2. Limiting the problem to a binary ‘flop’ or ‘success’ case, how accurate are the revenue predictions?

To answer these questions I will use three different algorithms:
* AdaBoost
* XGBoost
* LightGBM

I will use RMSE (root mean squared error) to determine the performance of each model.

## File Description <a name="description"></a>
This projects includes one Jupyter notebook with all code required for analyzing the data and creating a supervised machine learning algorithm. The csv file train.csv contains 3,000 movies with 22 variables as the training data set for the algorithm. The csv file test.csv contains the test data with 4,398 movies and 22 variables.

## Results
The main findings of the analysis have been published on [Medium](https://medium.com/@julia.nikulski/predicting-movie-revenue-with-adaboost-xgboost-and-lightgbm-262eadee6daa). A short overview of the results shall be given here:

1. Which variables are particularly predictive of absolute revenue figures?

* popularity
* budget
* budget_year_ratio
* release_year
* runtime
* title_length
* tagline_length
* release_week

2. Limiting the problem to a binary ‘flop’ or ‘success’ case, how accurate are the revenue predictions?

Converting the absolute values to a binary class system (flop or success) only leads to an accuracy of 68% in the cross-validation set.


## Licensing, Authors, Acknowledgements <a name="licensing"></a>
The data used for the analysis comes from [The Movie Database](https://www.themoviedb.org/documentation/api) and has been supplied by kaggle [here](https://www.kaggle.com/c/tmdb-box-office-prediction). There is licensing information on the datasets [here](https://www.themoviedb.org/documentation/api/terms-of-use) and [here](https://www.kaggle.com/c/tmdb-box-office-prediction). Feel free to use the code as you please and play around with it.
