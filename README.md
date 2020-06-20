# udacity-dsnd-project4
Udacity Data Science Nanodegree Project 4 (Capstone) - Predicting Churn for Sparkify App

### Table of Contents

1. [Project Overview](#overview)
2. [Data Descriptions](#data)
3. [File Descriptions](#files)
4. [Results and Discussion](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)


## Project Overview<a name="overview"></a>

This project implements [PySpark](https://spark.apache.org/docs/latest/api/python/index.html) to predict churn for a fictional music-streaming app, called Sparkify. Since this problem involves a large dataset, deploying on a cloud platform such as AWS or IBM cloud makes it possible to run the analysis without running into memory errors. This project involves synthesizing a number of different data science tasks, including:
 - *exploratory data analysis and visualization*: since we are given a new dataset without a whole lot of background, a large component of this project is getting a sense of this data and teasing out useful and irrelevant pieces in order to better predict churn
 - *data cleaning*: another important task is cleaning the data - removing null values and un-labeled users, etc.
 - *feature engineering*: once we've gotten a sense for the data and an idea of which variables appear to be more related to churn, we can create features that we'll use in the model
 - *model pipeline*: once we've cleaned the data and engineered some relevant features, the modeling aspect is pretty straightforward -- we will build some machine learning pipelines that assemble and scale the numerical features, and run the model
 - *model evaluation*: since this is an unbalanced dataset, the F1 score (harmonic mean of precision and recall) is better suited for this particular case
 - *model tuning*: finally once we have some baseline models, we can use cross-validation to find the best model parameters, and take a look at feature importances to include only what is needed 

### Problem Domain 

Predicting churn (customer attrition) rates is a common business problem, particularly in subscription-based business models that are increasingly common in our tech-driven world. Fortunately, many companies also collect a large amount of data from their users, including records of the customer's interaction with the app and all the app features. From this data, it is possible to predict which users are more likely to churn, and potentially preempt their cancellation by offering promotions, or addressing issues that may have increased the likelihood of churn. While python, and specifically the pandas library, have a slew of tools for running this sort of analysis on smaller datasets, it is often not enough for large datasets. The Spark framework handles the 

## Data Descriptions <a name="data"></a>
  
  1) `mini_sparkify_event_data.json`: a small subset of the data (128MB) used to test `PySpark` on a local machine (I ran all the analysis in the Udacity classroom environment)
  2) ``: 

## File Descriptions <a name="files"></a>

The repository contains a single jupyter notebook `Sparkify.ipynb` in which the analysis is carried out, based off the template provided in the Udacity workspace. There is a table of contents at the beginning of this notebook that can be used to get to each section.

## Results and Discussion<a name="results"></a>

Since my currrent line of work is in aerial mapping and environmental research, I am not as familiar with this sort of business analysis. I did some preliminary research to try and better understand different factors that might play into churn -- this [altexsoft business blog](https://www.altexsoft.com/blog/business/customer-churn-prediction-for-subscription-businesses-using-machine-learning-main-approaches-and-models/) was particularly useful as a starting point. 

Exploratory Data Analysis was a key component to this project - converting the `pyspark` dataframes into `pandas` dataframes, and using the `seaborn` plotting package, I was able to determine some variables from the Sparkify dataset that looked to be related to churn. Specifically the page column contained a lot of potentially useful information -- the figure below shows how churn is related to interactions with various pages, highlighting variables that have low and high correlation with churn. These features ended up being key components in the model. 

![Caption.](image.png)

In the modeling section 




## Licensing, Authors, Acknowledgments <a name="licensing"></a>
