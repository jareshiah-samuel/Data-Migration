# Data-Migration
Data Migration and Transformation Tool for Amazon RDS Data Warehouse

modules  to be imported :
import requests
import zipfile
import os
import pandas as pd
import boto3
import json
from sqlalchemy import create_engine
from sqlalchemy import text

Downloading the Zip File:
Use Python's requests library to download the zip file from the provided URL.
Save the zip file locally.

Extracting JSON Files from the Zip:
Utilize Python's zipfile library to extract the JSON files from the downloaded zip file.
Store the extracted JSON files in a temporary directory.

Storing Data in Amazon S3:
Use the boto3 library to interact with Amazon S3.
Establish a connection to your S3 bucket.
Upload the processed JSON data to the bucket

Loading Data into Amazon RDS:
Use Python's pymysql library to establish a connection to your Amazon RDS database.
Create the necessary table(s) in the database.
Insert the processed data into the appropriate table(s).

