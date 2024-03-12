# Spotify-Data-Engineering

### Introduction
In this project, I built an ETL (Extract, Transform, Load) pipeline using the Spotify API on AWS. The pipeline will retrieve the data from the Spotify API, transform it into our desired format, and load it into the AWS data store.

### Architecture
![Architecture Diagram](https://github.com/ninopadilla13/Spotify-Data-Engineering/blob/main/Spotify%20Data%20Pipeline.jpg)


### About Dataset/API
This API contains information about music artist, albums and songs.


### Services Used
1. **S3 (Simple Storage Service):** is an object storage built to store and retrieve any amount of data from anywhere.

2. **AWS Lambda:** is a serverless, event-driven compute service that lets you run code for virtually any type of application or backend service without provisioning or managing servers.

3. **Cloud Watch:** is a monitoring service for Amazon Web Services cloud resources and the applications you run on Amazon Web Services. You can use Amazon CloudWatch to collect and track metrics, collect and monitor log files, set alarms, and automatically react to changes in your Amazon Web Services resources.

4. **Glue Crawler:** is a fully managed extract, transform, and load (ETL) service that helps you to prepare and load your data for analytics.

5. **Data Catalog:** is an inventory of all the data that an organization collects and processes.

6. **Amazon Athena:** is a serverless, interactive analytics service that provides a simplified and flexible way to analyze petabytes of data where it lives.


### Install Packages
```
pip install pandas
pip install numpy
pip install spotipy
```

### Project Execution Flow
Extract Data from API -> Lambda Trigger (every hour) -> Run Extract Code -> Store Raw Data -> Trigger Transform Function -> Transform Data & Load It -> Query Using Athena



