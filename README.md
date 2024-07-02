# Ukraine Financial Aid - Support Tracker 
## An Overview of Military, Financial and Humanitarian Aid to Ukraine from both EU and non-EU Government 

Last update - 1st quarter of 2024

## 1) Introduction
### Which countries help Ukraine and how?
The Scope of Work of this project is to conduct an exploratory data analysis on the official IFW KIEL dataset for the Russo-Ukrainian War, regarding the military, financial and humanitarian support by governments to Ukraine since February 2022. By analyzing various faces of the dataset, including how the differents aid are spread, the spread-overtime and more insights, we seek to analyze how the 41 countries (42 with the EU) contributed. 

NOTE: Note: Allocations are specific aid packages have been delivered or earmarked for delivery to Ukraine. Due to lack of reliability, this analysis does not consider private donations or transfers by international organizations (Red Cross, Unicef et similar).

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
- Excel - Initial data cleansing, addressing formatting inconsistencies and improvment of data quality. Spacing and spreading of table.
- BigQuery Studio SQL - Data Cleaning and Analysis
- Tableau - Data Visualization for Dashboard
  
## 3) Data Analysis
### Exploratory Data Analysis (EDA) - Questions and findings

1) Who are the Top 10 Donors?
<details>
  <summary>See the findings</summary>
Bottom right chart focuses on top 10 donors by total allocations (each country split by category). They are shown as it's displayed here below:

| Donor                    | Total (B €) | Financial (B €) | Humanitarian (B €) | Military (B €)     |
|--------------------------|-------------|-----------------|--------------------| -------------------|
| EU                       | 77.11       | 74.82           | 2.29               | 0                  |
| United States            | 70.38       | 24.61           | 24.61              | 43.24              |
| Germany                  | 23.06       | 1.41            | 3.05               | 18.61              |
| United Kingdom           | 15.89       | 6.08            | 0.59               | 9.22               |
| Denmark                  | 8.77        | 0.13            | 0.24               | 8.40               |
| Japan                    | 7.81        | 5.69            | 2.05               | 0                  |
| Canada                   | 7.73        | 4.56            | 0.38               | 2.79               |
| Norway                   | 7.49        | 3.39            | 0.35               | 3.75               |
| France                   | 6.81        | 0.80            | 0.36               | 5.65               |
| Netherlands              | 6.21        | 1.06            | 0.72               | 4.44               |

*Range of Data available from 1/24/2022 to 2/29/2024*

As we can see, EU is the top donor "Country". Both EU and Japan donated a total of 0B for military aid (which is pretty understandable, especially from EU). Highest amount comes from US, standing out as 43.24B.
  
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
We can see, in the top 10 donor, a dominancy of Nothern-Europe region, and so:
  
| Country    | Share of GDP (%) |
|------------|------------------|
| Estonia    | 1.45             |
| Denmark    | 1.29             |
| Lithuania  | 1.14             |
| Latvia     | 1.07             |
| Finland    | 0.69             |
| Poland     | 0.64             |
| Slovakia   | 0.59             |
| Sweden     | 0.51             |

*Leading donors in terms of share of their GDP.*


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
  <img src="https://github.com/matteoproietti1/Ukraine_Aid/assets/169601063/ff1ebf13-ccc2-415d-854d-911ce33f9e2c" alt="Ukraine AID - Overview" width="1000">
  <p>As we can see, the top right chart refers to the distribution of aid throughout the years, with the very high peak in 06/2023 (2024 is still running so it cannot be fully taken into account). For more comprehensive insight, please refer to the calculation and interactive add-ons.
