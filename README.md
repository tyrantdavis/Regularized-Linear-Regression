# Regularized Linear Regression

## [Demo](https://nbviewer.org/github/tyrantdavis/Regularized-Linear-Regression/blob/main/LinearRegression-Boston.ipynb)

## Introduction
This project aims to extend the use of the simple linear regression house valuation model to analyze housing data from Boston, Massachusetts, particularly around various attributes for the homes observed in the area and their prices using multiple algorithms.

This project will scope, analyze, prepare, plot data, and seek to explain the findings from the analysis.

Here are a couple of questions that this project has sought to answer:

- Which algorithm performs best?
    - Ridge regression
    - Lasso regression
    - Elastic regression
- Which attribute has the greatest correlation to price?
- Which attribute has the least correlation to price?
- What emergent patterns seem to exist?


### Scenario
The goal is to use the house valuation models on datasets beyond those in the King County listings. A dataset with information about homes in Boston, Massachusetts has been discovered. This new data will help to create a model that predicts a home's value in this region based on various factors. However, relying solely on simple linear regression may not be the most effective solution for this issue. The desire is to avoid problems related to overfitting the model to the training data, which would hinder its ability to generalize to unseen data. Therefore, implementing regularization techniques into the linear models to help streamline the models and mitigate overfitting is a great idea. Instead of simply selecting one type of regularization method, all three options (ridge, lasso, and elastic net) will be assessed to determine which method meets the performance criteria best.

**Data Sources:**

- data/BostonHousing.csv
- [StatLib Archive](https://lib.stat.cmu.edu/datasets/boston)
- [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/)

## Project Goals
In this initiative, the viewpoint will be that of a real estate analyst. The analyst aims to predict housing prices with precision and efficiency. As a result, the primary goals will be to understand the features of homes and their corresponding prices, identify the attributes that have the most and the least significant impact on a home's price, and uncover emerging trends related to housing prices and location. Several questions will be asked:

- Which algorithm performs best?
    - Ridge regression
    - Lasso regression
    - Elastic regression
- Which attribute has the least correlation to price?



#### Why use a linear regression algorithm to produce a real estate price estimator?
A: The purpose of the model is to predict the price at which a house with particular attributes will sell. This is a regression type of outcome. While other algorithms can also produce a regression outcome, linear regression is simple, relatively easy to implement, and can produce a good result in many cases.

The house's median value(**Target**) will be the output (the dependent variable). The model will determine (predict) the
price through multiple inputs (independent variables). This seems like an appropriate task for a
regression model.

## Data
An anonymized dataset that can be used to train the machine-learning model has been found. It is a CSV file containing more than 506 real estate transactions in Boston, Massachusetts. 


## Conclusions

- Which algorithm performs best?
    - **Elastic regression** had the lowest MSE thus it performed the best in this situation, but only slightly better than a linear simple regression.

- Which attribute has the greatest correlation to price?
    - **RM** - the average number of rooms per house has the strongest positive correlation
      
- Which attribute has the weakest correlation to price?
    - **CHAS** - land bounds the Charles River

* What emergent patterns seem to exist? 
    * The houses in the area are considerably old.
    * Most houses are near employment centers.  
    * NO2 levels seem to vary, but the majority are generally low.  
    * The distribution of the number of rooms appears to be approximately symmetrical. 
    * The average number of rooms in a hose is six. Max is approximately 9 minimum about three and one-half
    * Generally speaking, the more rooms a house has the higher the median value
