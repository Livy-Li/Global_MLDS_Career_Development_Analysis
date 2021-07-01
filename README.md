# Global Machine Learning and Data Science Career Development Analysis

## Part 1. Statistical Analysis
### Dataset

Kaggle has hosted an open data scientist competition in 2020 titled “Kaggle ML & DS Survey Challenge.” The purpose of this challenge was to “tell a data story about a subset of the data science community represented in this survey, through a combination of both narrative text and data exploration.” More information on the competition, data, and prizes can be found on: https://www.kaggle.com/c/kaggle-survey-2020/data

The dataset provided (kaggle_survey_2020_responses.csv) contains the survey results provided by Kaggle. The survey results from 20036 participants are shown in 355 columns, representing survey questions. Not all questions are answered by eachparticipant, and responses contain various data types. In the dataset for the project, column Q24 “What is your current yearly compensation (approximate $USD)?” contains a numerical target variable. Rows with null salaries have been dropped (Please refer to **clean_kaggle_data.csv**).

### Summary

The objective of this part is to explore the survey data to understand

1. The nature of women's representation in Data Science and Machine Learning
2. The effects of education on income level. 

The analysis starts off by performing exploratory data analysis to analyze the survey dataset and to summarize its main characteristics. Graphical figures that represent trends in the data are presented. Then for each of the topic, descriptive statistics are extracted for every analyzed group. The income averages across groups are compared using appropriate statistical tests on both the original data and the bootstrapped data, in order to determine if the difference between groups are significant.

## Part 2. Salary Bucket Prediction
### Dataset

The dataset provided (kaggle_survey_2020_responses.csv) is preprocessed (please refer to clean_kaggle_data_2020.csv). Specifically, rows with the null values of salaries have been dropped. In addition, two columns ("Q24_Encoded" and "Q24_buckets") has been added at the end. Column "Q24_buckets" (Target Variable) have been obtained by combining some salary buckets in the column "Q24". Column "Q24_Encoded" has been obtained by label encoding the column "Q24_buckets".

### Summary

The purpose of this part is to train, validate, and tune **multi-class ordinary classification models** that can classify, given a set of survey responses by a data scientist, what a survey respondent’s current yearly compensation bucket is.

The development of the model includes steps below:

1) Handling missing values
2) Encoding variables
3) Analyze feature importance
4) Feature engineering and feature selection
5) Model implementation and hyperparameter tuning
6) Testing


