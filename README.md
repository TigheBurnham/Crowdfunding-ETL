# Crowdfunding-ETL

## Overview

Based on the previous SQL analysis Independent Funding received a new dataset that contained more information regarding the backers who’ve pledged to the crowdfunding projects. Therefore, Independent Funding requested a new ETL process to be performed on the updated dataset. In this analysis Python, Pandas, and Jupyter Notebooks were utilized to extract and transform the data through four different stages.

## Review

### Deliverable 1: Extract Data 

In this stage Python, Pandas, and Jupyter Notebooks were utilized to upload the backer csv file and create a new dataframe by iterating through each row and using list comprehension to append each row to a list. Below is a snippet of the list values for each row.

![Unclean_lists](https://user-images.githubusercontent.com/112028534/199880923-19b83971-9d27-4f71-8a89-a8db864359d0.PNG)

A new data frame was created through the list, and extracted to a backers.csv file.

### Deliverable 2: Transform and Clean Data

Next challenge was to clean the data frame through utilizing regex to parse out specific values from the backers info. For example we extracted the backer_id, cf_id, name, and email from the backer info column, and then split the new name column into last and first names. Since the backer's info and name columns were redundant they were dropped to clean the data. Below is a snippet of the clean dataframe.

![Clean_Backers](https://user-images.githubusercontent.com/112028534/199880901-b64d0f95-b104-48f6-b1b1-85f01992dc54.PNG)

### Deliverable 3: Create an ERD and a Table Schema and Load the Data

In this stage we imported the backers.csv created earlier and then updated the crowdfunding ERD diagram to look like the image below.

![crowdfunding_db_relationships](https://user-images.githubusercontent.com/112028534/199880492-e088e8e7-9405-4c4e-986c-ed895bef4206.png)

Next we updated the Schema to include the baker's table. Below is a table of the baker's table being successfully imported into the SQL Database.

![Backers_10_Rows](https://user-images.githubusercontent.com/112028534/199880481-18e63ac0-274c-4c6e-bca3-9807b4e3cdca.PNG)

### Deliverable 4 Requirements

In this deliverable the goal was to count the number backers for each campaign id, and then export two tables that captured the emails for the remaining contacts and backers as well as their funding goal amounts. These two new SQL tables were exported as csv files.

## Summary
In conclusion, the goal of this project was to teach the Extraction, Transformation, and Loading process and to demonstrate how important it is for data analysts in today's world especially when aiding stakeholders and helping them achieve their respective goals.
