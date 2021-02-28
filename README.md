# Capstone Project

## Purpose of this project

This is a supervised learning classification project on time-series data. The purpose of this project is to demonstrate my abilities to analyse a dataset and build a model to predict user churn of a music streaming service called Sparkify.

Note that two datasets are available: a full dataset of 12GB, that requires the deployment of a cluster to parallelize computation, and a mini-dataset of 128MB. In this repository the focus is on the mini-dataset for now. But note that due to the nature of this data, we wrote all the code using the Spark Framework to allow easy refactoring on the code to have it run with clusters on a much larger dataset.

In this repository, you will find a Jupyter notebook that goes through the process of:

- Exploring the data
- Engineering features
- Building a machine leaning classification model.

If you want to know more about the analysis on this projects and get more information you can read the article I wrote about this project [here](https://patonv.medium.com/sparkify-churn-analysis-a8b6a60ffde9)


## Requirements
The code is written in Python 3.7 with the Spark Framework (version 2.4.4).

The libraries use are:

- pandas
- numpy
- pyspark
- plotly
- os
- datetime
- seaborn

## Steps:

1. Load and Clean Dataset
2. Exploratory Data Analysis
3. Define Churn
4. Explore Data
5. Feature Engineering
6. Modeling:
    - Baseline Model
    - Random Forest
    - Supported Vector Machine
    - Gradient Boosted Trees

## Conclusion

### Summary
In this notebook, we implemented a model trying to predict customer churn. We removed rows with no userId, converted timestamp to a human readable format. 8 features were built for our model. We selected 3 models: GBM, SVM and RF to compare and select RF as the final model implemented for predicting final result. We used cross validation and grid search to fine tune our model. We achieved about 82% accuracy, and 78% F1 score, which is about 20% improvement compare to our baseline model (to consider everyone as not churn). Also, even though the accuracy drop from 83% to 82%, the F1 that indicates the presition improves.

### Improvement
The features can be improved a lot after considering more factors, adding more domain knowledges and expertise. Although the volume of data may required tools such as spark to analyze, but we can use more data to have better results as the user base grow.

Currently, we have about 225 records of unique users, and we only use 70% of them to train. That said, the model has a huge potential to improve if the sample size increase, and the expected performance will also increase.

## Acknowlegments and related content
The dataset (available [here](https://eu-west-2.signin.aws.amazon.com/oauth?SignatureVersion=4&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJEABXKD7P4LVZGHQ&X-Amz-Date=2021-02-23T15%3A43%3A23.620Z&X-Amz-Signature=398d45afdaa928bf9093a601587ec77947875a2c844a42022bc7f3f7f27f3d74&X-Amz-SignedHeaders=host&client_id=arn%3Aaws%3Aiam%3A%3A015428540659%3Auser%2Fs3&code_challenge=3g5SMbIsZKu1-LulNdaOIhwBwD3Us3uPlC_AsPo7UgE&code_challenge_method=SHA-256&redirect_uri=https%3A%2F%2Fs3.console.aws.amazon.com%2Fs3%2Fbuckets%2Fudacity-dsnd%2Fsparkify%2F%3Fregion%3Deu-west-3%26state%3DhashArgs%2523%26tab%3Doverview%26isauthcode%3Dtrue&region=eu-west-3&response_type=code&state=hashArgs%23&tab=overview)) used in this project was provided by Udacity. This is the capstone project for Udacity's Data Scientist Nanodegree.
