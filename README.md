# Capstone Project

## Purpose of this project

This is a supervised learning classification project on time-series data. The purpose of this project is to demonstrate my abilities to analyse a dataset and build a model to predict user churn of a music streaming service called Sparkify.

Note that two datasets are available: a full dataset of 12GB, that requires the deployment of a cluster to parallelize computation, and a mini-dataset of 128MB. In this repository the focus is on the mini-dataset for now. But note that due to the nature of this data, we wrote all the code using the Spark Framework to allow easy refactoring on the code to have it run with clusters on a much larger dataset.

In this repository, you will find a Jupyter notebook that goes through the process of:

- Exploring the data
- Engineering features
- Building a machine leaning classification model.


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

## Acknowlegments and related content
The dataset (available [here](https://eu-west-2.signin.aws.amazon.com/oauth?SignatureVersion=4&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJEABXKD7P4LVZGHQ&X-Amz-Date=2021-02-23T15%3A43%3A23.620Z&X-Amz-Signature=398d45afdaa928bf9093a601587ec77947875a2c844a42022bc7f3f7f27f3d74&X-Amz-SignedHeaders=host&client_id=arn%3Aaws%3Aiam%3A%3A015428540659%3Auser%2Fs3&code_challenge=3g5SMbIsZKu1-LulNdaOIhwBwD3Us3uPlC_AsPo7UgE&code_challenge_method=SHA-256&redirect_uri=https%3A%2F%2Fs3.console.aws.amazon.com%2Fs3%2Fbuckets%2Fudacity-dsnd%2Fsparkify%2F%3Fregion%3Deu-west-3%26state%3DhashArgs%2523%26tab%3Doverview%26isauthcode%3Dtrue&region=eu-west-3&response_type=code&state=hashArgs%23&tab=overview)) used in this project was provided by Udacity. This is the capstone project for Udacity's Data Scientist Nanodegree.
