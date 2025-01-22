# Sports-Analytics-Data-Lake-Using-Python-And-OpenSource

"Analytics and Insights"

# Technical Architecture

![image_alt](https://github.com/Tatenda-Prince/Sports-Analytics-Data-Lake-Using-Python-And-OpenSource/blob/78db69e24c02179bb1112636209649c125768ea2/images/Screenshot%202025-01-22%20153605.png)

## Project Overview

The nba_data_lake.py script performs the following actions:

Creates an Amazon S3 bucket to store raw and processed data. Uploads sample NBA data (JSON format) to the S3 bucket. Creates an AWS Glue database and an external table for querying the data. Configures Amazon Athena for querying data stored in the S3 bucket.

## Project Objectives

1.Store the raw nba data in json format in S3

2.Use AWS Glue to intergrate or transport and create a database table from our S3 bucket that will enable for athena to run SQL queries from our S3 bucket.

3.Use Athen Athena to query the data in S3 to find the information we need. 

## Background

## Amazon S3

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.



## AWS Glue 

AWS Glue is a serverless data integration service that makes it easy for analytics users to discover, prepare, move, and integrate data from multiple sources. You can use it for analytics, machine learning, and application development. It also includes additional productivity and data ops tooling for authoring, running jobs, and implementing business workflows.


With AWS Glue, you can discover and connect to more than 70 diverse data sources and manage your data in a centralized data catalog. You can visually create, run, and monitor extract, transform, and load (ETL) pipelines to load data into your data lakes. Also, you can immediately search and query cataloged data using Amazon Athena, Amazon EMR, and Amazon Redshift Spectrum.

## Amazon Athena 

Amazon Athena is an interactive query service that makes it easy to analyze data directly in Amazon Simple Storage Service (Amazon S3) using standard SQL. With a few actions in the AWS Management Console, you can point Athena at your data stored in Amazon S3 and begin using standard SQL to run ad-hoc queries and get results in seconds.


## Prerequisites

Before running the script, ensure you have the following:

1.Go to Sportsdata.io and create a free account At the top left, you should see "Developers", if you hover over it you should see "API Resources" Click on "Introduction & Testing"

2.Click on "SportsDataIO API Free Trial" and fill out the information & be sure to select NBA for this tutorial

3.You will get an email and at the bottom it says "Launch Developer Portal"

4.By default it takes you to the NFL, on the left click on NBA

5.Scroll down until you see "Standings"

6.You'll "Query String Parameters", the value in the drop down box is your API key.

7.Copy this string because you will need to paste it later in the script

8.IAM Role/Permissions: Ensure the user or role running the script has the following permissions:

S3: s3:CreateBucket, s3:PutObject, s3:DeleteBucket, s3:ListBucket Glue: glue:CreateDatabase, glue:CreateTable, glue:DeleteDatabase, glue:DeleteTable Athena: athena:StartQueryExecution, athena:GetQueryResults

## Technologies

1.loud Provider: AWS CloudShell Console 

2.Programming Language: Python 3.x

3.Core Services : S3 , AWS Glue and Amazon Athena 

4.IAM Security: Custom least privilege policies to allow access to our S3

5.Linux 

## Use Case 

You work at "Up The Chelsea" sports and they need someone to run analytics and insights for the NBA upcoming game and you are tasked with the responsibility to analyze an S3 Datalake holding NBA Data which can be queried to return relevant information for analytics and insights for the BOSTON TEAM.


## Step 1: Open CloudShell Console/ Local linux environment with AWS CLI installed 

1.Go to aws.amazon.com  and sign into your account

2.In the top, next to the search bar you will see a greater than square with a >_ inside, click this to open the CloudShell

## Step 2: Create the nba_data_lake.py file

1.In your the CLI (Command Line Interface), type

```language
nano nba_data_lake.py
```

2.Clone the repository
``` language

```



