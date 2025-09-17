# Spotify End-To-End Data-Engineering-project

### Introduction
In this project, I built an ETL(Extract, Transform and Load) pipeline using Spotify API on AWS. The pipeline retrieve data from Spotify API, transform it to a desired format, and load it into AWS Data store.

### Architecture
![Architecture Diagram](https://github.com/Douglasjr14/Spotify_end-to-end-data-engineering-project/blob/main/diagram.png)

### About Dataset/API

This API contains information about music artist, albums and songs.
[Sppotify API](https://developer.spotify.com/documentation/web-api)
 
### Services Used
1. **S3 (simple Storage Services)**: Amazon S3 is a highly scalable object storage service that can store and retrieve any amount of data from anywhere on the web. It is commonly used to store and distribuite large media files, data backups, and static website files.
2. **AWS Lambda**: AWS Lambda is a serverless computing service that lets you run your code without managing server. You can use Lambda to run code in reponse to events in S3, DynamoDB, or other AWS services.
3. **CloudWatch**: Amazon CloudWatch is a monitoring service for AWS resources and the applications you run on them. You can use CloudWatch to collect and track metrics,collect and monitor log files, and set alarms.
4. **Glue Crawler**: AWS Crawler is a fully managed service that automatically crawls your data sources, identifies data formats, and infers schemas to create an AWS Glue Data Catalog.
5. **Data Catalog**: AWS Glue Data Catalog is a fully managed metadata repository that maes it easy to discover and manage data in AWS. You can use Glue Data Catalog with others AWS services, such as Athena.
6. **Amazon Athena**: Amazon Athena is an interactive query service that makes it easy to analyse data in Amazon S3 using standard SQL. You can usa Athena to analyse data in you Glue Data Catalog or in other S3 Buckets.

### Install packages

```
pip install pandas as pd
import spotipy
import sys
from spotipy.oauth2 import SpotifyClientCredentials
```
