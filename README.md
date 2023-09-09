# Analysis of Airbnb Data using PostgreSQL

This repository contains SQL queries to analyze Airbnb data using a PostgreSQL database. The steps taken in the project are as follows:

1.I downloaded the dataset from Airbnb's official website. The biggest challenge I encountered was transferring this dataset to a PSQL database. I solved this using a Python script I wrote. I connected to the database using the SQLAlchemy library and performed the import of CSV files.

2.The dataset contains 72,332 records. Unnecessary columns that are irrelevant to the analysis were removed from the dataset, and rows with missing data in the remaining columns were deleted. The issue with currency symbols in the 'Price' column was resolved by creating a new column with numeric values.

3.With an SQL query, I listed the top 20 Airbnb hosts with the highest monthly earnings in the Istanbul region. I also ranked the hosts who received the most "negative" feedback and those who received the most "perfect" feedback.

4.With this work, Airbnb can provide pricing recommendations to hosts in Istanbul. Hosts with cleanliness issues in their homes can be alerted, and hosts who receive extremely positive feedback from users can be identified and rewarded.

## Data Source
You can download the data named listings and reviews for the desired region from the link below.
http://insideairbnb.com/get-the-data/

## Contents
- `python/`: Python scripts for importing the data to PostgreSQL
- `queries/`: SQL queries for analyzing the data
- `results/`: Results have been uploaded as 3 CSV files. Based on the results, analyses can be conducted on which hosts to prefer or not, which Airbnb hosts to reach out to for improvement discussions and increasing customer satisfaction, and finally, which hosts have prices that are too high or too low compared to the average, and how potential customer loss can be prevented.
-----------------------------------------------
Below is a simple visualization created with PostgreSQL, which can be further detailed with Power BI
![num_of_dirty_reviews](https://user-images.githubusercontent.com/110420596/229288285-b6e9d229-4d29-4c69-af7a-b7099a7c019f.png)
![num_of_perfect_reviews](https://user-images.githubusercontent.com/110420596/229288287-37f1573e-2165-4150-9cbd-8aef2a4c2858.png)
![top20](https://user-images.githubusercontent.com/110420596/229288288-1391e348-0c3f-4b87-ae7b-4e58792f3445.png)


## Credits
This project was completed by Burak Mustafa Karakaya as a personal project and is being included in my portfolio.

