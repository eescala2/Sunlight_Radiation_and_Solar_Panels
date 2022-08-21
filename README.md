# Target-Solar-Panel-Market-in-Michigan

# Overview 

Michigan is among the top one-sixth of states in per capita residential energy use, but the state's total energy use per capita is below the U.S. average. The residential sector is the leading energy-consuming sector, accounting for 30% of the state's energy use, followed closely by the transportation sector at 25%, the industrial sector at 24%, and the commercial industry at 22. Renewable energy accounted for about 11% of Michigan's total in-state electricity net generation in 2021. Most of the state's renewable electricity comes from wind, and customer-sited solar photovoltaic (PV) facilities provide almost 50% of the state's total solar power. In 2021, utility-scale (1 megawatt or more extensive) solar installations generated less than 1% of Michigan's total in-state electricity.

With the increasing interest and incentives from the federal government to increase the use and generation of renewable energy, there is a need to develop a model that will help predict the residential solar system count in Michigan. The goal of this project is to use data analytics tools, and a machine learning model to build a prediction model of residential solar system count in Michigan based on demographic trends in the following counties: Alpena, Calhoun, Genesee, Gogebic, Grand Traverse, Ingham, Kent, Mackinac, Oakland, Washtenaw, and Wayne. The demographic trends used in this project are median income, educational level (=> Bachelor level), homeownership percentage, and population density. 

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


### Prediction Model 
