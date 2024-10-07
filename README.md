# Project Background
 The State of New York Mortgage Agency (SONYMA) provides financing and programs designed for first-time low- and moderate-income homebuyers in New York State. The purpose of this analysis is to extract valuable insights from the dataset obtained from SONYMA, with the goal of providing recommendations to improve efficiency in loan distribution.

## Data Structure & Initial Checks
SONYMA’s database structure as seen below consists of 1 table, with 14 columns, a total row count of 28500 records. It includes raw data on all the loans purchased by SONYMA from January 2004 until 2016. It includes types of loans (loan amount, loan type, term, LTV, with or without down payment assistance), when the loans were made (purchase date), where the loans are being made (county), and what property types (# of units, construction status, property type).
![SONYMA columns](https://github.com/user-attachments/assets/5a89b725-443f-48b6-a8c1-9fe85b495eb2)

To see the Data dictionary, press [here](https://github.com/Tsatsaa8800/SONYMA-Loan-project/blob/main/HCR_SONYMALoanPurchased_DataDictionary.pdf)

## Data Preprocessing
### Data Cleaning in Excel:
The dataset was first imported into Excel, where initial cleaning was conducted. This included identifying and replacing abnormal values and removing 37 duplicate entries to ensure data consistency and integrity.

### Data Filtering and Querying:
SQL queries were used to filter and analyze the data, identifying patterns and summarizing key metrics for further analysis.

## Data Analysis and Visualization
  •	Complex SQL queries were executed to extract insights and prepare the dataset for visualization.
  
  •	The cleaned and processed data was then visualized using Tableau, where interactive dashboards were created to highlight key insights
  
Insights and recommendations are provided on the following key areas:

  •	[*Sales Trend Analysis*]: Evaluation of historical sales patterns over the years, and year to date focusing on loan amount, region, property type etc.
  
  •	[*Loan performance Analysis*]: Analysis on loan distribution by region and property type
  
  •	[*Down Payment Assistance Analysis*]: An evaluation of the usage of down payment assistance programs (CCAL & DPAL). 
  
  •	[*Regional Analysis*]: An evaluation of loan amount and down payment assistance by region
  
The SQL queries utilized to prepare data for the dashboard can be found [here](https://github.com/Tsatsaa8800/SONYMA-Loan-project/blob/main/SONYMA%20SQL%20QUERIES.txt)

An interactive Tableau dashboard can be downloaded [here](https://public.tableau.com/app/profile/tsatsral.ganzorig/viz/Propertyloan_Finalish/Dashboard2)

## Executive Summary

### Overview of Findings

After peaking in 2008, the Agency’s loan sales amount has been declining, with a significant drop of 65% from 2012 and 2014. Key performance indicators have all shown year-over-year decreases: Total loan amount by 22%, Loan-to-Value ratio by 23%, and down payment assistance loan amount by 17%. While this decline could be a sign of households cannot afford to buy a property due to a property value increase or lack of knowledge about down payment assistance program, the following sections will explore additional contributing factors and highlight key opportunities for improvement. 

Below is the overview page from the Tableau dashboard and more examples are included throughout the report. The interactive Tableau dashboard can be downloaded [here](https://public.tableau.com/app/profile/tsatsral.ganzorig/viz/Propertyloan_Finalish/Dashboard2)

![Screenshot 2024-10-04 183923](https://github.com/user-attachments/assets/2afebed2-62e3-4630-99bb-c4ca11bcdcf6)

 ## Sales trends: 
 
  •	The trend in loan amount over the years shows continuous decline while property values keep rising. 
  
  •	There is a notable -22.90% decrease in total loan amounts year over year (YOY). This decline suggests a potential slowdown in mortgage sales or lending activity, possibly due to factors like rising interest rates, stricter lending requirements, or decreased demand in the housing market.
  
  •	The LTV ratio has also dropped by -23% compared to last year, meaning buyers may be borrowing less compared to the value of the properties they are purchasing. This could indicate tighter credit conditions or more conservative borrowing behavior.
  
   •	The difference in loan amounts in areas suggest regional variations in property sales, with certain areas possibly experiencing stronger demand for loans (and therefore more property sales) than others.
   
   •	The total CCAL/DPAL amount also shows a decline of -17.7% from the previous year, which could suggest that fewer buyers are taking advantage of down payment assistance programs. However, certain counties have higher CCAL/DPAL amounts, potentially indicating stronger support or need for these programs in those areas.
   
## Key Findings

•	There is a correlation between loan amounts and property values over time, though the divergence since around 2013 suggests that property values have remained high while loan amounts have decreased.

•	The total loan amount in 2016 (current year) stands at $184.8M, marking a notable -22.90% decline year-over-year (YOY). This indicates a reduction in mortgage loan activity, potentially due to market conditions like higher interest rates or economic uncertainty.

•	The total amount for CCAL/DPAL (down payment assistance) is $3.5M, showing a -17.7% YOY decline. This decrease indicates lower engagement or availability of down payment assistance programs, potentially affecting first-time homebuyers who rely on these products.

•	Detached properties account for 78.41% of all loans, making them the dominant property type in the mortgage market. Condominiums (11.67%) and cooperatives (3.98%) represent smaller shares, with manufactured homes at only 0.40%.

•	Loan distribution by county varies significantly. Some counties, such as those with $188.1M and $99.6M in loans, show strong activity, while others have much lower loan amounts, indicating that mortgage loan performance is geographically uneven.

•	The CCAL/DPAL distribution varies widely by county, with some regions like the one having $9.4M showing strong demand for down payment assistance programs. Other counties have lower engagement with these programs.

## Recommendations
**[Launch region-specific marketing campaigns]**

o	Utilize detailed market analysis and local data to understand the factors affecting regional disparities in loan product performance

o	Offer incentives or tailored loan packages that meet the local economic conditions in these areas. For instance, in counties with high property values, offer premium loan packages, while in lower-performing areas, provide incentives or flexible terms.

o	Conduct borrower education campaigns using educational workshops, online resources, and partnerships with financial advisors to guide potential homebuyers on how to maximize their loan opportunities.

**[Increase promotion of down payment assistance programs]**

o	Partnership with real estate agents, financial advisors, and housing nonprofits. 

o	Simplify the application process to encourage more users

o	Consider introducing new benefits to make the program more attractive

**[Consider developing niche loan products for property types like condominiums and cooperatives to diversify the portfolio and cater to growing urban markets]**

**[Reevaluate loan terms to potentially increase the maximum LTV ratio for qualified buyers, making loans more accessible and affordable]**

o	Consider offering additional incentives for borrowers with strong credit histories, such as lower interest rates or relaxed down payment requirements.

o	Review lending policies to ensure they match current property values. Adjust maximum loan amounts or loan-to-value ratios to better reflect property price growth, enabling borrowers to take on higher loans that align with their property purchases.



