# IT-Salary

## Project Goals
This project is to highlight the different techniques that can be used to improve on a linear model. By linear model, it emcompasses the class of all Generalized Linear Models (GLMs) as well as polynomial extensions. As linear regression is a relative simple model with hardly any hyperperimeter to tuning, these techniques will require working around the model, modifying the features in order to raise scores.

## Data Collection
The data is from a survey of the [income of IT professionals](https://www.kaggle.com/parulpandey/2020-it-salary-survey-for-eu-region) in Europe and it is available at Kaggle. Some of the features in this datasets are:

- position
- total years of experience
- seniority level
- main technology / programming language

## Data Cleaning
There are some missing data and the values are easily imputed using KNN imputer. I checked for outliers of salary but did not find justifiable reason to remove all of them. However, I did remove a few of observations where the salary is over 1 million euros. I expanded out some features, like 'other programming languages' and drop a few features that are not relevant to predicting salary.

## Model Building
The linear models in this project include linear regression, ridge regression, huber regression, gamma regression and tweedie regression. I also extended the model with polynomial features and target transformer. I compared categorical features that are one-hot encoded with ones that are smart encoded using the category encoder library.
