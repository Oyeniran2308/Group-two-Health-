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

 **Fig 1** 
 
![My_project final 11_22_2024 11_02_27 AM](https://github.com/user-attachments/assets/07cfc8b9-2471-40aa-9d0a-3098d3dea4a5)

![My_project final 11_22_2024 9_27_43 PM](https://github.com/user-attachments/assets/93428764-32df-4eee-93d5-56679dbbca19)


**Date Function:** Date_Table = CALENDARAUTO()

## COVID-19 Mortality Analysis Across Regions

**- Region with the Highest COVID-19 Deaths**
  Approximately 32.9 million deaths were recorded across all regions, of which 3.4 million deaths (10.3%) were attributed to COVID-19. Among all regions, the United States reported the highest    number of COVID-19 deaths, with 1,011,492 cases accounting for 12.0% of the global COVID-19 mortality. Notably, January emerged as the most severely affected month, recording 178,058 deaths.

**Fig 1.**
  ![population across region](https://github.com/user-attachments/assets/67b295e5-4efa-42aa-91c4-e9e6f1fd444b)

**- Peak COVID-19 Mortality Trends**
  The analysis reveals that COVID-19 deaths reached their peak in 2021, with a total of 1,654,330 deaths (12.1%). January was the deadliest month in 2021, with 320,900 deaths, while June recorded the lowest monthly deaths at 66,100.

**Fig 2.**
![covid and non-covid death per year](https://github.com/user-attachments/assets/328df46e-1abe-4596-b55e-7e78a8e688dc)

**- Total COVID-19 and Non-COVID Deaths**

   COVID-19 Deaths: Approximately 3.4 million deaths were attributed to COVID-19 across 46 regions.

   Non-COVID Deaths: A total of 29.5 million deaths were non-COVID-related, signifying that the majority of fatalities in these regions were not linked to the pandemic.

**Fig 3**
![covid and non-covid death per year](https://github.com/user-attachments/assets/f9692fa8-3b2f-43fc-9eec-d07f76959d93)

**- Correlation Between Expected Deaths and COVID-19 Deaths**

   Analysis of expected deaths versus COVID-19 deaths indicates: The highest recorded COVID-19 deaths were 35,153, with other significant values being 63,320 and 62,940.
   For the subgroup 59,442, COVID-19 deaths accounted for 1.04%.
   Across 5,673 expected deaths, COVID-19 deaths ranged from 0 to 35,153, demonstrating no clear correlation between expected deaths and COVID-19 mortality.

**Fig 4**
![expected and covid death](https://github.com/user-attachments/assets/fb28be51-9fcf-4e4e-82ba-e06a931cff3d)

  _This analysis highlights critical patterns in COVID-19 mortality, emphasizing the United States' disproportionate impact, the temporal peaks in 2021, and the distinction between COVID and       non-COVID-related fatalities._

## Findings

**Monthly Analysis of Expected Deaths:**

_January recorded the highest expected deaths, with a total of 3,445,863, which is 108.61% higher than September, the month with the lowest expected deaths at 1,651,847._
_Expected deaths showed a positive correlation with COVID-19 deaths, suggesting that periods with higher COVID deaths also tended to have higher expected death counts._
_January accounted for 12.12% of the total expected deaths for the period analyzed._
_The greatest divergence between expected deaths and COVID-19 deaths occurred in January, with expected deaths exceeding COVID deaths by 2,928,231._

**Range of COVID-19 Deaths by Country:**

_Across the 46 countries analyzed, COVID-19 deaths ranged significantly, from a minimum of 121 deaths to a maximum of 1,011,492 deaths._

**Yearly Analysis of COVID-19 Deaths:**

_The year 2021 had the highest total COVID-19 deaths, with 1,654,330 deaths, which is 225.45% higher than 2022, the year with the lowest total of 508,319 COVID-19 deaths._
_COVID-19 deaths showed a positive correlation with non-COVID deaths, indicating that years with higher COVID-19 fatalities also had an increase in non-COVID deaths._
_2021 accounted for nearly half (48.92%) of the total COVID-19 deaths for the time period covered._

**Divergence Between COVID and Non-COVID Deaths:**

_The largest difference between non-COVID and COVID-19 deaths was observed in 2020, with non-COVID deaths surpassing COVID deaths by 11,070,337._

**Range of Deaths by Region:**

**COVID-19 deaths across regions varied widely, with values ranging from 121 to 1,011,492 deaths, while non-COVID deaths ranged from 5,758 to 7,395,917 deaths.*


## Recommendations

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

## Conclusion

This dashboard effectively captures the stark impact of COVID-19 on global mortality. However, the 
dominance of non-COVID deaths (89.7%) suggests an urgent need to address broader health challenges 
beyond the pandemic. By identifying hotspots and trends, policymakers can design targeted 
interventions to reduce preventable deaths, improve global health equity, and prepare for future crises
