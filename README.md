## **Ken Noppinger**

**COVID-19 Study**

This research investigates the prevalence of COVID-19 in the most densely populated places in the US. 

Since March 2020, the COVID-19 virus has been raging through the US and around the world. To date, there are over 50 million cases worlwide and over 10 million cases within the US.  During the spring, it was learned that the virus can be spread airborne through droplets and since that discovery there has been a significant emphasis placed on social distancing and wearing masks by health organizations and both state and federal governments. This analysis will shed light on the impact of 
population density relative to the virus spread.  

The goal is to determine which densely populated places in the US have done a better job of containing the spread of the virus.

---
**Key Questions**

1. What counties in the US are the most populated?
2. What counties in the US are the most densely populated?
3. What counties in the US have the most confirmed cases of COVID-19?
4. Are the most densely populated counties represented in the counties with the highest case counts?  If not, which ones?
5. How do case counts in densely populated counties compare to counts in densely infected counties?  Is there a correlation?

---
**Data Sources**

<u>Daily COVID-19 Reports</u>

The following COVID-19 data file will be referenced from the Johns Hopkins Resource Center at Github (note - the file is updated daily):
- https://github.com/CSSEGISandData/COVID-19/blob/master/csse_covid_19_data/csse_covid_19_daily_reports/10-23-2020.csv

<u>Population Data</u>

The following file provides population estimates for all counties in the US (note - 2019 estimates will be used):
- https://www.ers.usda.gov/data-products/county-level-data-sets/download-data/PopulationEstimates.xls

<u>Land Area Data</u>

The following census data file will be used to extract the county land area information needed for the study:
- https://www.census.gov/library/publications/2011/compendia/usa-counties-2011.html

<u>GEOJSON Data</u>

The following GEOJSON file contains the polygon definitions for counties by FIPS code and the data is used in generating choropleth maps.
- https://raw.githubusercontent.com/plotly/datasets/master/geojson-counties-fips.json

<u>COVID-19 Time Series Data</u>

The following COVID-19 data file will be referenced from the Johns Hopkins Resource Center at Github (note - the file is updated daily):
- https://github.com/CSSEGISandData/COVID-19/blob/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_US.csv


---
**Units & Variables**

The main unit for analyis is a "county" in the US.  There are over 3000 counties that will be used in the study.

Key variables or metrics to the study are:
- County Population
- County Land Area (Sq. Miles)
- County Population Per Square Mile
- Confirmed Cases (aggregate)
- Confirmed Cases Per Square Mile
- New Confirmed Cases by Month

---
**Algorithm**

The Jupyter Notebook is broken into a three parts:
- Part I - Data Loading, Cleaning, and Merging
- Part II - Answering Questions
- Part III - Additional Visualization

<u>Part I - Data Loading, Cleaning, and Merging</u>
- Read and Clean COVID-19 Daily Report
- Read and Clean Population Data
- Merge COVID-19 and Population Data by FIPS code (i.e., county)
- Read and Clean Land Area Data
- Merge Land Area and COVID/Population Data
- Define Charting Functions (to support analysis)

<u>Part II - Answering Questions</u>
- Answer Key Questions 1 through 5
- Use horizontal bar charts, scatter charts, and histograms to visualize data in supporting answers to the questions

<u>Part III - Additional Visualization</u>
- Visualize County Data on Choropleth Maps
  - Display a Population Density Choropleth Chart
  - Display a Case Density Choropleth Chart 
- Investigate COVID Time Series Data
  - Read and Clean COVID-19 Time Series Data
  - Create Monthly Buckets for New COVID-19 Cases
  - Display Charts Showing New Cases Per Month

<u>Conclusion</u>
- Summary of findings

---
