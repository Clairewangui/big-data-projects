# Real-Time Twitter Sentiment Analysis

## Overview
This repository contains a Big Data project focused on real-time sentiment analysis of Twitter data (classification of tweets).  
The project leverages various technologies to collect, process, analyze, and visualize sentiment data from tweets in real-time.

---

## Architecture
The project is built using the following components:

- **Apache Kafka**: Used for real-time data ingestion from Twitter dataset.  
- **Apache Spark Streaming**: Processes the streaming data from Kafka to perform sentiment analysis.  
- **MongoDB**: Stores the processed sentiment data.  
- **Django**: Serves as the web framework for building a real-time dashboard to visualize the sentiment analysis results.  
- **Chart.js & Matplotlib**: Used for plotting and visualizing sentiment trends.

---

## Project Structure
Real-time Data Ingestion: Collects live tweets using Kafka from the Twitter DataSet.
Stream Processing: Utilizes Spark Streaming to process and analyze the data in real-time.
Sentiment Analysis: Classifies tweets into different sentiment categories (positive, negative, neutral) using natural language processing (NLP) techniques.
Data Storage: Stores the sentiment analysis results in MongoDB for persistence.
Visualization: Provides a real-time dashboard built with Django to visualize the sentiment trends and insights.
## Features

- **Real-time Data Ingestion**: Collects live tweets using Kafka from the Twitter dataset.  
- **Stream Processing**: Utilizes Spark Streaming to process and analyze the data in real-time.  
- **Sentiment Analysis**: Classifies tweets into different sentiment categories (positive, negative, neutral) using natural language processing (NLP) techniques.  
- **Data Storage**: Stores the sentiment analysis results in MongoDB for persistence.  
- **Visualization**: Provides a real-time dashboard built with Django to visualize the sentiment trends and insights.

## Description 

In This Project I'm using a Dataset (twitter_training.csv and twitter_validation.csv) to create pyspark Model and for create live tweets using Kafka. Each line of the "twitter_training.csv" learning database represents a Tweet, it contains over 74682 lines;

The data types of Features are:

- **Tweet ID**: int
- **Entity**: string
- **Sentiment**: string (Target)
- **Tweet content**: string

The validation database “twitter_validation.csv” contains 998 lines (Tweets) with the same features of “twitter_training.csv”.

This is the Data Source: https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis

## Structure

- **Django-Dashboard**: Contains the Django web application for the real-time dashboard.  
- **Kafka-PySpark**: Contains Kafka producer scripts and PySpark streaming jobs (Kafka consumer).  
- **ML PySpark Model**: Contains the trained ML model, Jupyter notebooks, and datasets.  
- **zk-single-kafka-single.yml**: Docker Compose file to set up Apache Kafka and Zookeeper.  
- **bigdataproject_rapport**: A brief report about the project (in French).
