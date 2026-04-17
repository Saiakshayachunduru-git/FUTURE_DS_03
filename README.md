# FUTURE_DS_03
📊 Bank Marketing Funnel Analysis Project Report
1. Project Title

Bank Marketing Campaign – Data Extraction & Funnel Analysis

2. Objective

The objective of this project is to analyze a bank marketing dataset to understand:

Customer conversion behavior
Overall campaign effectiveness
Conversion rate of term deposit subscriptions
3. Tools & Technologies Used
Python 🐍
Pandas (for data handling)
Zipfile (for handling compressed datasets)
4. Dataset Description

The dataset is stored inside a nested ZIP file structure:

Outer file: bank+marketing.zip
Inner file: bank.zip
Final dataset: bank-full.csv

The dataset contains marketing campaign data such as:

Customer demographics
Campaign contact details
Previous marketing outcomes
Target variable: y (subscription to term deposit: yes/no)
5. Methodology
Step 1: Data Extraction
Opened the main ZIP file using zipfile.ZipFile
Extracted the inner ZIP file (bank.zip)
Loaded the CSV file (bank-full.csv) directly without extracting manually
Step 2: Data Loading
Read dataset using pandas.read_csv()
Used separator ; as required by dataset format
Step 3: Data Cleaning
Converted target column y:
yes → 1
no → 0

This made the dataset suitable for numerical analysis.

Step 4: Funnel Analysis

Calculated:

Total number of customers contacted
Number of customers who subscribed
Conversion rate percentage
6. Key Code Logic (Summary)
ZIP handling using Python’s built-in zipfile
Nested ZIP extraction (ZIP inside ZIP)
Data transformation using Pandas mapping
Simple business KPI calculation (conversion rate)
7. Results
📌 Total Customers Contacted: len(df)
📌 Total Conversions: df['y'].sum()

📌 Conversion Rate:

Conversion Rate=
Total
Converted
	​

×100

This gives a clear idea of how effective the marketing campaign was.

8. Outcome
Successfully extracted and analyzed nested ZIP dataset
Converted raw data into meaningful business insights
Calculated key marketing KPI: Conversion Rate
9. Conclusion

This project demonstrates how Python can be used for:

Real-world data extraction from compressed files
Data preprocessing and transformation
Basic marketing analytics and funnel analysis

It provides useful insights into customer conversion behavior in bank marketing campaigns.
HERE IS A SNAPSHOT OF  THE RESULT:
<img width="763" height="422" alt="image" src="https://github.com/user-attachments/assets/4903aa23-6ed2-4570-ac14-9d45e66ab273" />

