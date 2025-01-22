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


