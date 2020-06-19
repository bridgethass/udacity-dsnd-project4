# udacity-dsnd-project4
Udacity Data Science Nanodegree Project 4 (Capstone) - Predicting Churn for Sparkify App

### Table of Contents

1. [Project Overview](#overview)
2. [Data Descriptions](#data)
3. [File Descriptions](#files)
4. [Results and Discussion](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)


## Project Overview<a name="overview"></a>

This project implements PySpark to predict churn for a fictional music-streaming app, called Sparkify. This involves synthesizing a number of different data science tasks, including:
 - *exploratory data analysis and visualization*: since we are given a new dataset without a whole lot of background, a large component of this project is getting a sense of this data and teasing out useful and irrelevant pieces in order to better predict churn
 - *data cleaning*: another important task is cleaning the data - removing null values and un-labeled users, etc.
 - *feature engineering*: once we've gotten a sense for the data and an idea of which variables appear to be more related to churn, we can create features that we'll use in the model
 - *model pipeline*: once we've cleaned the data and engineered some relevant features, the modeling aspect is pretty straightforward -- we will build some machine learning pipelines that assemble and scale the numerical features, and run the model
 - *model evaluation*: since this is an unbalanced dataset, the F1 score (harmonic mean of precision and recall) is better suited for this particular case
 - *model tuning*: finally once we have some baseline models, we can use cross-validation to find the best model parameters, and take a look at feature importances to include only what is needed 
 - *(py)spark*: this is all implemented using pyspark library framework, so that it can be deployed on a cloud platform

### Problem Domain 

Predicting churn (customer attrition) rates is a common business problem, particularly in subscription-based business models that are increasingly common in our tech-driven world. Fortunately, many companies also collect a large amount of data from their users, including records of the customer's interaction with the app and all the app features. From this data, it is possible to predict which users are more likely to churn, and potentially preempt their cancellation by offering promotions, or addressing issues that may have increased the likelihood of churn. While python, and specifically the pandas library, have a slew of tools for running this sort of analysis on smaller datasets, it is often not enough for large datasets. The Spark 

## Data Descriptions <a name="data"></a>
  
  1) `mini_sparkify_event_data.json`: a small subset of the data used to test PySpark on a local machine (in the Udacity classroom environment)
  2) ``: 

## File Descriptions <a name="files"></a>

The repository contains the following files:

    1) Sparkify.ipynb - this notebook contains exploratory data analysis including the following components:
        - 
    2) ...

## Results and Discussion<a name="results"></a>


## Licensing, Authors, Acknowledgments <a name="licensing"></a>
