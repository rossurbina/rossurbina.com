# Global Climate Changes to Temperature, Disasters, & CO2 Emissions Over Time

## Overview
### Purpose
I wanted to explore how climate change has impacted temperature change and the number of disasters (outputs) over time. I also wanted to explore the relationship of how factors that influence climate change (inputs), such as CO2 emissions, affect temperature change and disasters. Finally, I analyzed countries’ inputs and outputs by region and income level to see how they contribute to and are affected by climate change.

### Data Tools Used
I used Python in Jupyter Notebook to clean, transform, and analyze the data. I then exported csv files from Jupyter Notebook into Tableau, where I visualized the data. The Python code is in Github, and the Tableau dashboard link is https://public.tableau.com/app/profile/ross.urbina/viz/GlobalClimateVisualizationProject/Dashboard1


## Insights & Observations
### Main Conclusion
The average temperature change and disasters per country in each income bracket is generally the same and the trends are similar. However, the CO2 emissions produced varies dramatically based on the country’s wealth. This shows that while the high income countries are the main ones responsible for CO2 emissions, all countries face same or similar effects on temperature change and disaster.

### Detailed Conclusions

**TEMPERATURE CHANGE SINCE 1960:** No material difference of temperature change based on either the income level or region; temperature rises are highly correlated

**DISASTERS SINCE 1980:** No significant differences of percentage increase of disasters based on either the income level or region

**CO2 POLLUTION PER CAPITA SINCE 1900**

  **Income level:** CO2 emissions are directly related to the income group, with the high income having the highest emissions and low income having the lowest. The 1950s was the peak of CO2 emissions for high income countries with 20, which has since dropped to around 9. 
  
  •	Upper middle income countries today have the same CO2 emissions as high income countries in 1940

  •	Lower middle income countries today have 20% less emissions today than high income countries did in 1900
  
  **Region:** North America has always emitted the most CO2 per capita, except from 1950-1965 when Latin America skyrocketed its emissions and 1991 in MENA (likely data error). Since then, Latin America’s emissions have reduced dramatically. 

**TYPES OF CO2 SINCE 1900**

**Growth percentage:** From 1900 to 2021, the percentage growth each year from CO2 emissions was 2.48%

**Percentage breakdown of CO2 type:** every type of CO2 has generally risen each year but at different growth rates. The biggest 3 contributors are coal (41%), oil (30%), and gas (22%)

## Steps to Data Analytics Process

### Explore & Gather Data
I used 6 different databases for this analysis. Below are the links to each data source: 

•	Temperature change: https://climatedata.imf.org/datasets/4063314923d74187be9596f10d034914 

•	Disasters: https://climatedata.imf.org/datasets/b13b69ee0dde43a99c811f592af4e821/explore 

•	Forest & Carbon: https://climatedata.imf.org/datasets/66dad9817da847b385d3b2323ce1be57/explore 

•	Land: https://climatedata.imf.org/datasets/b1e6c0ea281f47b285addae0cbb28f4b/explore 

•	CO2 Population: https://ourworldindata.org/co2-and-greenhouse-gas-emissions 

•	Country Demographic Information: https://datatopics.worldbank.org/world-development-indicators/the-world-by-income-and-region.html 

### Cleaning & Transforming the Data with Python

•	Used melt function to transpose years from many columns to 1 row for each datset, which varied in number of columns

•	Cleaned string values by only gathering a word description, instead of 20+ words

•	Selected which attributes are most important for analysis, and merged all files together

•	Removed countries with at least one NaN value to not obscure the time series data

•	Normalized data for each country to compare land changes over time

•	Basic data cleaning / transformation (remove nulls, remove rows not in correct categories, divide population by 1M, etc.)

•	Transposed various CO2 types into 1 column to visualized them altogether

### Data Visualization (Tableau)

For all charts, I merged a dataset with region & income level of each country and created parameters & filters, so the viewer can filter on income level, region, & country in the dashboard. The following charts were created. Here is the link to the Tableau Dashboard: https://public.tableau.com/app/profile/ross.urbina/viz/GlobalClimateVisualizationProject/Dashboard1

•	Avg country temperature change by Income level

•	Average country Disasters by Income group

•	CO2 pollution Per 1M people by Income Group

•	Total CO2 Pollution by Type

•	Map view of temperature change (takes average change from 2018-2022 and compares with 1961 baseline)

•	Percentage change of Country’s Artificial Surfaces increase


