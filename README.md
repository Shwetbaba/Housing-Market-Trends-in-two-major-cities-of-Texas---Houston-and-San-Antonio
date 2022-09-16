# Project 2: Extract, Transform, Load 
## Housing Market Trends in two major cities of Texas - Houston and San Antonio
---
## Description
This project will be evaluating the housing market trends in Houston and San Antonio, Texas. The Team will evaluate the living preferences (renting vs owning) of persons currently living in Texas. We used multiple data sources to determine the best option of whether to rent or buy a property.

**Motivation**
There appears to be an increase in population in San Antonio and surrounding areas, as there are multiple housing and commercial structures being erected seemingly weekly. The purpose of this analytical research is to make the best decision with regards to renting vs buying. 
We will be extracting and examining data from areas in and around San Antonio and Houston to identify trends. This information can prove to be useful to new property developers, real estate investors, and persons relocating to those areas.
Is it more cost effective to rent vs buy a property?

## Analysis
**Extract**
i.	We extracted the data from sources using two methods via Pandas:
ii.	Extracting data from a CSV file (Zillow.com)
iii.	Web Scraping from Texas A&M: Texas Real Estate Research Center
iv.	Libraries utilized: 
•	Pandas, 
•	PyMongo, 
•	webdriver_manager.chrome
•	unicodedata - return Unicode string unistr in the normal form
•	splinter

**Transform:**
* Cleaned up the CSV and the HTML data in various ways including:
* Dropped columns
* Reassigned data types 
* String and Object conversion to Integer to allow for calculations on some columns
* Formatted/mapped strings to dollar format
* Filtered date range to match the evaluation period as determined by the team
* Our transformation allowed for us to filter data related to the cities in question: San Antonio and Houston.

**Load:**
We used a nonrelational database model to collect data on housing cost by region. We used MongoDB due to its flexibility and ease of use. We used Pandas dataframe to join our data from Houston and San Antonio utilizing data scraped from web prior to adding it to the database.

## Conclusion
Based on the data collected it is more cost efficient to own a home than it is to rent one based on the mortgage payment (not including taxes). This assumes that it is a long-term accommodation rather than a short-term living arrangement.

## Datasets Used:
* <a href="https://www.zillow.com/research/data/"> Zillow.com</a>
  * RENTALS Zillow Observed Rent Index (ZORI): Houston and San Antonio
* <a href="https://www.recenter.tamu.edu/data/housing-activity/#!/activity/MSA/Houston-The_Woodlands-Sugar_Land">Housing Activity for Houston-The Woodlands-Sugar Land</a>
  * Median Housing Price for the year 2021 for Houston Area
* <a href="https://www.recenter.tamu.edu/data/housing-activity/#!/activity/MSA/San_Antonio-New_Braunfels">Housing Activity for San Antonio-New Braunfels</a>
  * Median Housing Price for the year 2021 for San Antonio Area

## Files and Folders included:
* Jupyter Notebook 
  * HousingMarketAnalysis.ipynb
  
* Resources folder
  * Metro_zori_sm_month.csv

## Group 2 Team Members:
* Shwet 'Sunny' Bhatt - ETL Houston Housing Price information
* Waynette Burke - ETL San Antonio and Houston Rental Information
* Ariana Garcia - ETL San Antonio Housing Price Information