

![Image 1](https://user-images.githubusercontent.com/124645643/231342541-1cf93140-f650-41d1-9f5c-415827840a63.jpg)



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
- **Pandas Process:** With Pandas, we read the CSV files, parsed conditions using the loc function, transposed the data, used the groupby function to filter the industries and provinces, calculated the measures of central tendency using the aggregate function and also computed statistics for the provinces and industries.  We also calculated the average temperature changes for the different seasons in Quebec, Alberta and Ontario.

- **Matplotlib Process:** Using the previously created PANDAS data frames, we created additional layers to parse specific data and this included addition of supplemental groupby functions to organize this data. Once the data was organized we were able to create line and stacked bar graphs using pyplot.

- **API Process:** The dataset includes Canada temperature that contains climate changes in the different provinces over a period of time from 1989 – 2017. We parsed conditions using the loc function. The dataset was also grouped and sorted based on the season’s average temperature and GHC emissions in the different provinces. 


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

![Image 2](https://user-images.githubusercontent.com/124645643/231343250-ead898fc-565c-4747-b5ea-c850f7f27b27.png)
 
Canada’s gas emissions were initially within the set targets by the UN until after 2004 where Canadas’s emissions increased and exceeded the set gas emissions by the UN.


## 2.	Canada Emissions per Industry

 ![image 3](https://user-images.githubusercontent.com/124645643/231343268-dc7abe22-f053-4f66-a01e-9787257f1fef.png)
 
The Oil and Gas, Electricity and Transport Industries contributed more than 50% of the total GHG emissions in Canada.
 
 ## Three Main Industries of Focus
 
![Image 4](https://user-images.githubusercontent.com/124645643/231343281-fb46095e-e91d-4ae9-ae3d-b489b8b40fbe.png)

## 3.	Canada emissions per Province and Territory
 
 ![Image 5](https://user-images.githubusercontent.com/124645643/231343292-3cc79abf-416e-493f-bd15-7aa8c3c9d61b.png)
 
Ontario, Quebec and Alberta regions contribute more than 50% of the total emissions in Canada.
 
 ## Ontario emissions per Industry
 
 ![Image 6](https://user-images.githubusercontent.com/124645643/231343300-3c69a1d1-6271-4da8-a1e2-708f7839e5d5.png)
 
Oil and Gas Industry emissions in Ontario were almost constant during the period analyzed whereas the emissions from the Transportation industry increased. Notably, emissions from the Electricity industry have remarkably decreased.

## Alberta emissions per Industry

![Image 7](https://user-images.githubusercontent.com/124645643/231343309-fe8d8f36-8d6c-4b9a-a6f1-a1dec9f67cb6.png)

Alberta has the highest level of GHC emissions in Canada and this is mainly attributed to the Oil and Gas Industry contributing more than 50% on the emissions .
 
 ## Quebec emissions per Industry
 
 ![Image 8](https://user-images.githubusercontent.com/124645643/231343318-4704dad9-1bfa-40e5-b8f8-82dfc7423c88.png)
 
The Transportation Industry contributes more than 80% of Quebec’s GHC Emissions. 
 
 
## Temperature data per seasons in the 3 provinces of focus

## Alberta Temperature data per seasons
 
 ![image 9](https://user-images.githubusercontent.com/124645643/231343330-14bbbde2-8c05-47ff-ba28-0cc6ea7b2201.png)
 
 ## Ontario Temperature data per seasons
 
 ![image 10](https://user-images.githubusercontent.com/124645643/231343343-8347747d-bfba-4259-9811-229b2aaa9d5c.png)
 
## Quebec Temperature data per seasons
 
 ![image 11](https://user-images.githubusercontent.com/124645643/231343353-fa1b091a-3ce4-4fc5-a0cf-282a565a8e07.png)
 
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

- Another difficulty involved reading the UN API file which we decided to leave out and focus on the Canada weather API.  


## Conclusion
- Canada’s gas emissions were initially within the set targets by the UN until after 2004 where Canadas’s emissions increased and exceeded the set gas emissions by the UN.

- The Oil and Gas, Electricity and Transport Industries contributed more than 50% of the total GHG emissions in Canada.

- Population has a big impact on the levels of emissions realized in a given region. The Lesser populated regions registered low levels of emissions as opposed to the densely populated regions that exhibited high levels of emissions. 

- Oil and Gas Industry emissions in Ontario were almost constant during the period analyzed whereas the emissions from the Transportation industry increased. Notably, emissions from the Electricity industry have remarkably decreased.

- Alberta has the highest level of GHC emissions in Canada and this is mainly attributed to the Oil and Gas Industry contributing more than 50% on the emissions.

- The Transportation Industry contributes more than 80% of Quebec’s GHC Emissions.

- There is an increase in the average temperature and with the current emissions trend, temperatures are most likely to continue increasing. 











