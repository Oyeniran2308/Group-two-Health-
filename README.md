# ANALYSIS ON COVID-19 INFECTION ACROSS REGION
## Project Objective
The objective of this analysis is to examine the regional trends and impacts of COVID-19 by  analyzing infection rates, recovery rates, and mortality across different geographical areas.
## Table of Content
## Dataset
- Source: Kaggle (https://www.kaggle.com/datasets/dhruvildave/covid19-deaths-dataset)
- Size: 5770 rows, 10 columns
- Key Fields:

  1. Country & Region: geographical location of affected places
  2. Year
  3. Expected death
  4. Total Death
  5. Covid death
  6. Non-covid death
## Exploratory Data Analysis (EDA)
The exploratory data analysis (EDA) aims to address the following critical questions:

- Which region reported the highest number of COVID-19-related deaths?
- In which year did COVID-19 death counts reach their peak?
- What is the total number of COVID-19-related deaths recorded across all regions?
- What is the total number of non-COVID-related deaths recorded across all regions?
- How does the number of expected deaths correlate with COVID-19-related deaths when analyzed by the month of the end date?

These insights will provide a comprehensive understanding of the data trends and relationships related to COVID-19 mortality.

## Tools and Technique used

• Tools: Microsoft Excel , Power BI

• Techniques

**Data Cleaning:** Microsoft excel was used to remove duplicate, check blank space, change 
the case and align columns.
**Data Visualization:** Measure table was created ('Measures' = ROW("measures", 
BLANK()) and under measure table some measures which help in the analysis was also 
created.
- Percentage of Non covid death: % Non_Covid = ('''Measures'''[Non Covid_death]/ 
'''Measures'''[Total Death])
- Percentage of Excess death: % of excess death = ('''Measures'''[Total excess 
death]/'''Measures'''[Total Death])
- Percentage of covid death: %_of_Covid_death = ('''Measures'''[Covid 
Death]/'''Measures'''[Total Death])
- Covid Death = SUM(all_weekly_excess_deaths[covid_deaths] )
- No of country = DISTINCTCOUNT(all_weekly_excess_deaths[country])
- Non Covid_death = SUM(all_weekly_excess_deaths[non_covid_deaths])
- Total Death = SUM('all_weekly_excess_deaths'[total_deaths])
- Total excess death = SUM(all_weekly_excess_deaths[Excess Death])

**Date Function:** Date_Table = CALENDARAUTO()

## Recommendations:

**1. Regional Focus:**
- Regions with higher COVID death concentrations (e.g., Europe and North America) 
should be prioritized for further analysis, including healthcare infrastructure, population 
density, and vaccination rates.
- Efforts should also examine whether underreporting or limited healthcare access is 
skewing data in regions like Africa.

**2. Improving Data Accuracy:**
- Countries should standardize data collection and reporting mechanisms to ensure 
consistency across regions.
- Enhance tracking for comorbidities that might bridge the gap between COVID and nonCOVID deaths.

**3. Preparedness for Future Pandemics:**
- Insights from the data should guide policymaking for early detection, resource 
allocation, and public health strategies.

**4. Preventive Measures:**
- Strengthen vaccination programs, particularly in regions showing fewer reported cases 
but vulnerable populations.
- Promote health awareness campaigns to reduce the number of preventable non-COVID 
deaths.
