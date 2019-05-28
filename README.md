# wiki_scraper - TOPOS Data Engineering assignment
Write a scraper in either python or NodeJS to collect data from Wikipedia about the top cities in the United States. The fields you collect, as well as the volume of data is up to you, but ideally you add additional data beyond the initial table, such as data found on the individual city pages, or other sources of your choice. The final format should be a CSV file that is ready to be uploaded to a BigQuery table. Please read Bigquery’s Manual to prepare your CSV in the right format. Intermediary steps, environments or processes necessary to run the scraper should be documented in code as well as a Readme.md and hosted on github in a repo devoted to this assignment.

## About the project
This project scrapes the data from Wikipedia's page of 'List of United States cities by population' and creates a csv file. Apart from the data from the main table, this scraper also goes to each cities wiki link and adds extra information as well.
Information from the main table for each city in the table:
1. Rank
2. City
3. State
4. 2018 Estimate
5. 2010 Census
6. Change
7. 2016 Land Area Km
8. 2016 Land Area Mi
9. 2016 Population Density km
10. 2016 Population Density mi
11. Wiki link

Information added from their respective wiki links:
1. Land Area
2. Water Area
3. Time Zone
4. Mayor
5. Airport
6. Official Website
7. Climate

## Requirements
1. Python>3.6, pip and Jupyter Notebook. I would recommend using Anaconda to use Jupyter Notebook and create a conda environement to run this notebook. There are other ways to run this Notebook, eg: Google Colab
2. All the other necessary packages including beautifulsoup is mentioned at the start of the code and the notebook will download them if not found in the system

## Step:
Run the notebook and it will generate a required csv file titled "top_cities_US.csv" in the current working directory. It is ready to be uploaded to a BigQuery Table.
