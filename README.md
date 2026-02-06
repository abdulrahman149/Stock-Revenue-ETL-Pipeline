# Stock-Revenue-ETL-Pipeline

# Project Overview
This project demonstrates a complete data engineering pipeline: extracting historical revenue data for Tesla and GameStop using web scraping and API calls, performing data transformation in Python, and building a professional business intelligence dashboard to visualize growth trajectories.

# Technical Stack
Language: Python 3.x
Libraries: * BeautifulSoup & Requests (Web Scraping)
yfinance (Financial API)
Pandas (Data Cleaning & ETL)
BI Tool: IBM Cognos Analytics

# Data Workflow
1. Extraction: Utilized the yfinance library to extract historical stock prices.
    Built a custom scraper using BeautifulSoup to parse HTML tables for historical revenue data from static snapshots to ensure pipeline stability.
2. Transformation (ETL):
    Cleaned "Revenue" strings by removing currency symbols and commas using Regex.
    Standardized date formats and converted data types into numeric values for time-series analysis.
    Merged disparate datasets into a unified CSV for cross-company comparison.
3. Visualization:
    Exported cleaned data into IBM Cognos Analytics.
    Designed a dashboard featuring line charts for growth trends and clustered column charts for direct year-over-year competition analysis.

# Key insights
  Tesla's Pivot: The dashboard highlights the specific inflection point where Tesla transitioned from linear to exponential revenue growth.
  Market Contrast: Visualizing GameStop's volatility alongside Tesla's growth provides a clear picture of shifting market sectors over the last decade.

# How to Use
1. Open the Web_Scraping.ipynb notebook to view the extraction logic.
2. Run the cells to generate the tesla_revenue.csv and gme_revenue.csv files.
