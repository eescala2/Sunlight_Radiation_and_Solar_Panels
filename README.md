# Target-Solar-Panel-Market-in-Michigan

![solar](Visuals/solar.png)

# Overview 

Michigan is among the top one-sixth of states in per capita residential energy use, but the state's total energy use per capita is below the U.S. average. The residential sector is the leading energy-consuming sector, accounting for 30% of the state's energy use, followed closely by the transportation sector at 25%, the industrial sector at 24%, and the commercial industry at 22. Renewable energy accounted for about 11% of Michigan's total in-state electricity net generation in 2021. Most of the state's renewable electricity comes from wind, and customer-sited solar photovoltaic (PV) facilities provide almost 50% of the state's total solar power. In 2021, utility-scale (1 megawatt or more extensive) solar installations generated less than 1% of Michigan's total in-state electricity.

With the increasing interest and incentives from the federal government to increase the use and generation of renewable energy, there is a need to develop a model that will help predict the residential solar system count in Michigan. The goal of this project is to use data analytics tools, and a machine learning model to build a prediction model of residential solar system count in Michigan based on demographic trends in the following counties: Alpena, Calhoun, Genesee, Gogebic, Grand Traverse, Ingham, Kent, Mackinac, Oakland, Washtenaw, and Wayne. The demographic trends used in this project are median income, educational level (=> Bachelor level), homeownership percentage, and population density. 

![key_figures](Visuals/key_figures.png)

# Analysis

Does income affect solar panel ownership?

![Avg  Number of Solar System_Median Income](https://user-images.githubusercontent.com/101475984/184557445-ecf6d96d-57d5-45ff-b29e-63a340a5457e.png)

Is solar radiation levels different based on region in Michigan?

![Avg  Number of Solar System _ Homeownership Rate](https://user-images.githubusercontent.com/101475984/184557454-039af6d1-146b-4346-a4fe-e9c8b4d35d63.png)

Do highly populated regions have more Solar Systems?

![Avg Number of Solar System _Educational Level](https://user-images.githubusercontent.com/101475984/184557498-96463900-f12c-46cc-84b8-9d9cec4637cb.png)

What is the average number of Solar Systems per region?

![Population Density](https://user-images.githubusercontent.com/101475984/184557581-e83b287f-0d91-40e9-8e10-62ab471f13c8.png)

# Machine Learning Model : Linear Regression 

Linear Regression is the supervised Machine Learning model in which the model finds the best fit linear line between the independent and dependent variable. 

![image](https://user-images.githubusercontent.com/101475984/185814717-4a65d521-3b63-45b2-98dc-83653ea58ce0.png)

Y= bo + b1X1 + b2X2 + b3X3 + b4X4

## Correlation Analysis 

![image](https://user-images.githubusercontent.com/101475984/185814784-23ad4c1f-da8f-4ccf-9905-0c63ca863812.png)

Based on the correlation level, the Solar System Count Residential is positively correlated with Median income, educational level, and homeownership. This means that if one of these variables decreases the solar system count residential will decrease. The population density is negatively correlated with the Residential Solar System count this indicates that if the population density increase the Residential Solar system count will decrease.

## Regression Results 

### R-Square 


### Variation Inflation Factor (VIF)

### Predicition Model

# Machine Learning Model

The preliminary data investigation began with the premise that we would have to collect three distinct types of data: household data regarding income, education, work experience, et cetera (other factors that could also affect and explain our analysis such as ethnicity), solar data for the state of Michigan (to be then divided by region), and installation of solar panels.  Household data was easily found through the American Community Survey database provided by the Census Bureau. After a preliminary investigationa and discussion, we decided to go with solar irradiance data from the NREL database using their web user interface where we collected data by county using coordinates.

The most difficult data to find was the installation of solar panels on households. Whereas the first two datasets were found within a few days, the last dataset was unable to be found until we discovered a Stanford dataset created through deep learning. The Stanford dataset observed satellite data by household to detect whether solar panel installtions were on the house. The data was then included in a master dataset that encompassed the whole country. For the purposes of this project, we removed all data not related to Michigan. We were also looking to include a temporal variable to see if there was any sort of change in adaption over the span of five years, however, the deep learning dataset was built in 2018 and thus only used data for that year. 

Our machine learning model is an ordinary least square linear regression. We are looking for the factors that influence adoptation of solar panels in a community. Variables that we are to include (subject to change) include household income, education, ethnicity, etc., solar irradiance data (whether the amount of sunlight in a region plays a factor in the adaptation in solar panels), region, population. 

Therefore our dependent variable would be the percentage of households with solar panel installations. Independent variables such as household income, education, ethnicity, solar irradiance data, location characteristics (whether it is urban or rural, or in a more northern region) will be tested to see which model has the highest r-squared value, along with the p-values of each variable.The r-square value will assist in validating the effectiveness of the model and whether it will help characterize the individual most likely to install solar panels.


# Dashboard

![Dashboard](Visuals/Dashboard.png)

https://public.tableau.com/app/profile/safari.nde/viz/TargetResidentialSolarPanelinMichigan/TargetSolarPanelMarketinMI?publish=yes

# Example Schema

![Schema](Visuals/Schema.png)

# Slides

https://docs.google.com/presentation/d/1LrtH7fWyHEKxciRR_yIGYUzSCKBZ0iV8DgcXWfFzEIY/edit?usp=sharing


# Resources

**Data:** 

Average Household Income MI - Census Bureau

Homeownership rate in MI - Census Bureau

Renewal Energy Sector in MI - Census Bureau

NREL National Solar Radiation Database 2015 - 2020

DeepSolar by Stanford - https://web.stanford.edu/group/deepsolar/home

# Communication Protocols

Team members collaborated using Zoom for meetings, Git Hub for subitting our work and Slack for all other communications outside of meetings. We also utilized Google Docs for an outline and Google Slides for the presentation.

