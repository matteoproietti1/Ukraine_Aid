# Ukraine Financial Aid - Support Tracker 
## An Overview of Military, Financial and Humanitarian Aid to Ukraine from both EU and non-EU Government 

Last update - 1st quarter of 2024

## 1) Introduction
### Which countries help Ukraine and how?
The Scope of Work of this project is to conduct an exploratory data analysis on the official IFW KIEL dataset for the Russo-Ukrainian War, regarding the military, financial and humanitarian support by governments to Ukraine since February 2022. By analyzing various faces of the dataset, including how the differents aid are spread, the spread-overtime and more insights, we seek to analyze how the 41 countries (42 with the EU) contributed. Due to lack of reliability, this analysis does not consider private donations or transfers by international organizations (Red Cross, Unicef et similar).

### Data Sources
The first part of the analysis regarded the collection of data. For this, many differents tables have been gathered from a single .csv file available at "INSERT LINK OF DATASET", and many outliers were not taken in consideration (mainly to avoid a too-in-depth analysis that would have caused confusion).
The datasets are: "allocations_delivery.csv", "allocations_overtime.csv", "allocations_group.csv", "comprehensive.csv".
The main data source is updated every quarter from the members of the Institute World Economy, which the Team are: Pietro Bomprezzi, Ivan Kharitonov, and Christoph Trebesch.

## 2) Data processing
### Data preparation
During the cleaning and preparation phase, following tasks were performed:
1) Creation of a Staging table to preserve the original data
2) Identification and removal of duplicates and outliers
3) Standardization of Data (formatting)
4) Handling missing and null values to avoid imprecise analysis

### Tools
- Excel - Initial data cleansing, addressing formatting inconsistencies and improvment of data quality.Spacing and spreading of table.
- BigQuery Studio SQL - Data Cleaning and Analysis
- Tableau - Data Visualization for Dashboard
  
## 3) Data Analysis
### Exploratory Data Analysis (EDA) - Questions and findings

1) Who are the Top 10 Donors?
<details>
  <summary>See the findings</summary>


  
</details>

2) Compare 2022 and 2023. How different is the distribution of Aid throughout the two years?
<details>
    <summary>See the findings</summary>



</details>

3) Diversification of aid. In what category appears to be the highest amount of donations?
<details>
  <summary>See the findings</summary>

 </details>

4) What country donated the most, considering the donation as a share of their GDP?

<details><summary>See the findings</summary>


</details>

5) What's the difference between total commitments and total allocations? Who has the highest deficit percentage yet to be allocated?

<details><summary>See the findings</summary>
The total committments are 259.14B.

Left to be allocated is 89.49B. Of those, the European Union has the biggest share of 57.75% (49.50B). Following: Germany, Uk and then...
</details>

### Visualization
From this analysis, the data available allow us to gather some more interest finding, summarized in the following dashboard, which the interactive version can be found on [Tableau Public](https://public.tableau.com/app/profile/matteo.proietti8500/viz/UkrainesConflict-1Qof2024update/Dashboard1). 

<details>
  <summary>View the Dashboard</summary>
  <img src="https://github.com/matteoproietti1/AirBnB_Analysis/assets/169601063/b8d20c94-ddaa-426e-a6f6-f0bf353e02d9" alt="Milan Visualization Overview" width="1000">
  <p>The Buenos Aires - Venezia neighborhood has the highest number of listings, with 1,475 in total. Andrea is the top host, owning 41 of these listings. The average price for an entire home in this neighborhood is 192 euros per night (25 euros more than the average price of a staying in Milan, which is 167 euro).
