## Twitter Sentiment Analysis with Tweepy, Azure Cosmos DB, Azure Databricks, and Power BI

---

This project aims to leverage the power of social media, particularly Twitter, to collect a vast amount of real-time data about public opinions and sentiments. We employ a suite of tools and technologies, including the Twitter API for data collection, Azure Cosmos DB for storage, Azure Databricks for data processing and analysis, and Power BI for visualization.

### Features

- Utilizes Tweepy, a Python library that simplifies the use of the Twitter API.
- Streams and collects real-time tweets with defined search rules (e.g., Premier League team names) using the Twitter API.
- Stores data securely and efficiently with Azure Cosmos DB.
- Employs Azure Databricks for powerful data processing and analysis.
- Leverages Power BI for intuitive data visualization.


## Objectives

The main objectives of our project are as follows:

1. **Real-time Twitter Data Collection**: Utilize Twitter API to collect real-time tweets. 

2. **Data Storage**: Store the collected tweets in a robust and scalable NoSQL database, Azure Cosmos DB.

3. **Data Analysis**: Leverage Azure Databricks, a distributed analysis platform based on Apache Spark, to analyze and process the data. Specifically, we plan to perform sentiment analysis on the tweets to determine the general opinion of Twitter users on specific topics.

4. **Results Storage**: Save the analysis results in a Hive Metastore for further access and analysis.

5. **Data Visualization**: Visualize the analysis results using Power BI. This enables end users to interact with the data and derive valuable insights.



## Getting Started

1. **Prerequisites**: Install the necessary Python packages.

2. **Twitter API Key**: You need to create a Twitter Developer account and generate API Keys to use the Twitter API.

3. **Azure Account**: You also need an Azure account for using Azure Cosmos DB and Azure Databricks.

4. **Running the Scripts**: Run `get_tweets.py` to start collecting tweets. Then run `Twitter-Databricks.py` in an Azure Databricks notebook to analyze the tweets.

5. **Power BI**: Connect Power BI to your Hive Metastore where your analysis results are stored to create visualizations.


## Repository Structure

- **README.md**: This document, a general introduction to the project and guide for users.

- **Twitter-Databricks.py**: The Python script used in Azure Databricks to analyze and process the tweets. It utilizes the transformer library to use a RoBERTa-based model for sentiment analysis.

- **get_tweets.py**: The Python script for collecting real-time tweets using Tweepy library and Twitter API. It streams tweets based on certain keywords and stores the data into Azure Cosmos DB.

- **databricks.png**: An image file showing the Azure Databricks notebook where the sentiment analysis is conducted.

### License

This project is licensed under the [ELFI](LICENSE).

---
