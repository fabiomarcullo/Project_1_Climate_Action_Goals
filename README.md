**Team Members:** Fabio Marcullo De Lima, Bruna Câmara, Annbell Nakigozi, Yamileth Cova, Rahiq Osman and Joseph Arambula


# CLIMATE ACTION GOALS – REPORT

## Executive Summary
Introduction: In June 1992, at the Earth Summit in Rio de Janeiro, Brazil, more than 178 countries adopted Agenda 21, a comprehensive plan of action to build a global partnership for sustainable development to improve human lives and protect the environment. Progress of these targets is tracked by the unique indicators. 

### Objective
This project aims to highlight SDG 13, the global climate action goal set by the UN in 1992 and analyzing the development of this goal by Canada as a country between the years 1992 and 2020, in order to understand whether this goal is being achieved by the Government of Canada and for each province separately.



## Data sources 
This project used the database CSV files below to create datasets regarding the trends overtime based on Greenhouse gas emissions for the UN and Canada’s provinces and industries. We also used the weather API CSV to create the temperature dataset showing the temperature trends overtime per season for the different provinces based on GHC and temperature. 

 The CSV files solely focus on SDG 13.2 .2” Total Greenhouse emissions per year.”
 
-	UN Database for the UN goals CSV file 
- Canada Database for Canada Economic sectors CSV file and Provinces Economic sector CSV file.
- Kaggle CSV file.



## Data Cleaning and Exploration
The data collected was transformed in order to analyze and visualize with Python using the following techniques:
- Pandas Process: With Pandas, we read the CSV files, parsed conditions using the loc function, transposed the data, used the groupby function to filter the industries and provinces, calculated the measures of central tendency using the aggregate function and also computed statistics for the provinces and industries.  We also calculated the average temperature changes for the different seasons in Quebec, Alberta and Ontario.

- Matplotlib Process: Using the previously created PANDAS data frames, we created additional layers to parse specific data and this included addition of supplemental groupby functions to organize this data. Once the data was organized we were able to create line and stacked bar graphs using pyplot.

- API Process: The dataset includes Canada temperature that contains climate changes in the different provinces over a period of time from 1989 – 2017. We parsed conditions using the loc function. The dataset was also grouped and sorted based on the season’s average temperature and GHC emissions in the different provinces. 


### Insights we had while exploring the data 
- Covid19 pandemic. We were surprised that the UN targets were not tracked in 2020 during the pandemic There was also a significant reduction in the emissions of C02 in Canada and all the industries in 2020. 

- GHC emissions have increased over the years as the lowest emissions were registered in the early nineties across the board. 

- Industry Analysis; Oil and Gas, Electricity and Transport Industries contribute more than 50% of the total emissions in Canada and this guided our focus of analysis on these three major industries.

- Provincial Analysis:
Population has a big impact on the levels of emissions realized in a given region. The Lesser populated regions registered low levels of emissions as opposed to the densely populated regions that exhibited high levels of emissions. 
Ontario, Quebec and Alberta regions contribute more than 50% of the total emissions in Canada and this also guided our focus of analysis on these three major provinces.   


### Challenges encountered while exploring that data 
- For Canada GHG Emissions per Province and Territory, the Northwest Territories and Nunavut were combined as one for the first decade analyzed, and then were separated in two different regions.

- Finding ways to make the graph as detailed and clean as we wished. And also, adjusting the colors, because, for example for the Canada GHG Emissions per Province, Matplotlib has a cap of 10 colors, so Yukon had the same color as Alberta, and Northwest Territories.

- Consolidating the multiple Data Frames into one.






## Summary Statistics


## 1.	UN GHG Target vs Canada GHG Emission

 
Canada’s gas emissions were initially within the set targets by the UN until after 2004 where Canadas’s emissions increased and exceeded the set gas emissions by the UN.





## 2.	Canada’s Sectors Gas Emissions 
 
The Oil and Gas, Electricity and Transport Industries contributed more than 50% of the total GHG emissions in Canada.
 


## 3.	Emissions by Canada Provinces. 
 
 
 
 
 
Oil and Gas Industry emissions in Ontario were almost constant during the period analyzed whereas the emissions from the Transportation industry increased. Notably, emissions from the Electricity industry have remarkably decreased.





Alberta has the highest level of GHC emissions in Canada and this is mainly attributed to the Oil and Gas Industry contributing more than 50% on the emissions .
 
 
 
 
The Transportation Industry contributes more than 80% of Quebec’s GHC Emissions. 
 
 
 
 
 
Temperature data per seasons in the 3 provinces of focus
 
 
 
## Questions addressed 
### Q1) Why we chose to SDG 13.
We prioritized SDG 13 because of the current climate change impacts, and the amount of data available, not only on the UN website, but also on the government of Canada website where we acquired most of our data.

### Q2) Canada’s level of attaining set targets vs UN targets
Canada’s gas emissions were initially within the set targets by the UN until after 2004 where Canadas’s emissions increased and exceeded the set gas emissions by the UN. This has been well illustrated in the UN GHG Target vs Canada GHG Emission graph. 

### Q3) Factors impacting Canada’s achievement of the targets.
Based on the Emissions of Canada per Industry graph, it was observed that the Oil and Gas, Electricity and Transport Industries contributed more than 50% of the total GHG emissions in Canada. 
The Oil & Gas sector comprises of emissions from natural gas production and processing, upstream oil and gas, Oil sands, crude bitumen mining and extraction, petroleum refining among others.
The Transport sector includes emissions from the different transport forms used (Road, Marine, Rail and Aviation), combustion emissions from off road and portable engines and other mobile related emissions including fossil fuels and non CO2 emissions from biofuels. 
The Electricity sector consists of combustion and process emissions from utility electricity generation, steam production (for sale) and transmission

## Limitations encountered
- We wanted to see how Canadian regulations evolved and its possible impacts on the GHG Emissions so we could create a similar graph, but we failed to obtain a data source so we could work on. Failure to exploit the UN API file.

- We were also planning to talk about target 13.a” *Implement the commitment undertaken by developed-country parties to the United Nations Framework Convention on Climate Change to a goal of mobilizing jointly $100 billion annually by 2020 from all sources to address the needs of developing countries in the context of meaningful mitigation actions and transparency on implementation and fully operationalize the Green Climate Fund through its capitalization as soon as possible* ” in a Canadian perspective but only world is available.

- Another difficulty involved reading the UN API file which we decided to leave out and focus on the weather API.  


## Conclusion
- Canada’s gas emissions were initially within the set targets by the UN until after 2004 where Canadas’s emissions increased and exceeded the set gas emissions by the UN.

- The Oil and Gas, Electricity and Transport Industries contributed more than 50% of the total GHG emissions in Canada.

- Population has a big impact on the levels of emissions realized in a given region. The Lesser populated regions registered low levels of emissions as opposed to the densely populated regions that exhibited high levels of emissions. 

- Oil and Gas Industry emissions in Ontario were almost constant during the period analyzed whereas the emissions from the Transportation industry increased. Notably, emissions from the Electricity industry have remarkably decreased.

- Alberta has the highest level of GHC emissions in Canada and this is mainly attributed to the Oil and Gas Industry contributing more than 50% on the emissions.

- The Transportation Industry contributes more than 80% of Quebec’s GHC Emissions.

- There is an increase in the average temperature and with the current emissions trend, temperatures are most likely to continue increasing. 











