# Retail Sales Data Analysis

## Overview
This project involves collecting, processing, and analyzing retail sales data from a web source. The analysis explores sales patterns, customer demographics, and product performance across different time periods.

## Project Structure
```
├── COMP47670-Assignment1-Task1.ipynb      # Data collection and scraping
├── COMP47670-Assignment1-Task2-3.ipynb    # Data preparation and analysis
├── sales_data.csv                         # Raw scraped data
├── cleaned_sales_data.csv                 # Processed dataset
├── README.md                              # Project documentation
└── images/                                # Visualizations and charts
```

## Data Collection (Task 1)
The first part of this project involved web scraping to collect retail sales data from `http://mlg.ucd.ie/modules/python/assignment1/retail/index.html`. The data collection process included:

- Identifying the URL structure (organized by quarters Q1-Q4, with multiple pages each)
- Using BeautifulSoup and requests to extract data from HTML tables
- Handling inconsistent formatting in customer details and dates
- Cleaning and standardizing the data (removing currency symbols, fixing date formats)
- Extracting customer information using regex patterns
- Saving the cleaned data to CSV format

## Data Preparation and Analysis (Task 2-3)
The second notebook focuses on further data preparation and exploratory analysis:

- Handling missing demographic values (creating "Unknown" categories)
- Converting dates to datetime format and extracting temporal features
- Creating age group categories for better demographic analysis
- Calculating profit margins
- Standardizing payment methods
- Visualizing monthly sales trends and other patterns

## Technologies Used
- Python 3.9
- Libraries: pandas, matplotlib, seaborn, BeautifulSoup, regex, requests
- Jupyter Notebook

## How to Run
1. Clone this repository
2. Install required packages: `pip install -r requirements.txt` (if you've created one)
3. Run the notebooks in order:
   - First `COMP47670-Assignment1-Task1.ipynb` to collect data
   - Then `COMP47670-Assignment1-Task2-3.ipynb` for analysis

