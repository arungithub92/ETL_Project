# Spar-Nord-Bank-ETL-Project

## Problem Statement

* In this project, Spar Nord Bank aims to enhance ATM cash management by closely monitoring withdrawal patterns and the associated influencing factors. 
* The objective is to optimize the frequency of cash refills, taking into account variables such as ATM activity, geographical location, weather conditions, and the day of the week.
* Additionally, the project seeks to extract valuable insights from the data beyond just refill frequency optimization.

## Data

* Spar Nord Bank has published this dataset at Kaggle under [Database Contents License (DbCL) v1.0 — Open Data Commons](https://opendatacommons.org/licenses/dbcl/1-0/).
* Source of the Data Set in Kaggle: [Kaggle Data Set](https://www.kaggle.com/sparnord/danish-atm-transactions)

## Approach

The project unfolds through a structured series of steps:

* Data ingestion from RDS to HDFS using Sqoop
* Reading the data from the files in HDFS by a specific schema using PySpark
* Creation of dimension tables using PySpark
* Creation of transaction fact table using PySpark
* Loading the dimension and fact tables into Amazon S3 bucket
* Creation of a Redshift Cluster
* Setting up a database in the Redshift cluster and running queries to create the dimension and fact tables
* Loading data into a Redshift cluster from Amazon S3 bucket
* Using queries on a Redshift cluster to find the solution to the following analytical queries.
