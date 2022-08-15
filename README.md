# Target Solar Panel Market in Michigan 

![solar](Visuals/solar.png)

# Overview

Our team is interested in discovering our target market for residential solar panels in specific reginal Michigan cities. With solar panels being the cheapest form of clean and renewalable engery, we are looking to focus on areas with ideal solar radiation and a minimum base income to ensure that solar panels are cost effective for the customer.


# Analysis

What is the average income for the region?

What is the average of homeownership in the region?

What is the average residential electric use based on region?

What is the average solar radiation output for the region?

# Machine Learning Model

The preliminary data investigation began with the premise that we would have to collect three distinct types of data: household data regarding income, education, work experience, et cetera (other factors that could also affect and explain our analysis such as ethnicity), solar data for the state of Michigan (to be then divided by region), and installation of solar panels.  Household data was easily found through the American Community Survey database provided by the Census Bureau. After a preliminary investigationa and discussion, we decided to go with solar irradiance data from the NREL database using their web user interface where we collected data by county using coordinates.

The most difficult data to find was the installation of solar panels on households. Whereas the first two datasets were found within a few days, the last dataset was unable to be found until we discovered a Stanford dataset created through deep learning. The Stanford dataset observed satellite data by household to detect whether solar panel installtions were on the house. The data was then included in a master dataset that encompassed the whole country. For the purposes of this project, we removed all data not related to Michigan. We were also looking to include a temporal variable to see if there was any sort of change in adaption over the span of five years, however, the deep learning dataset was built in 2018 and thus only used data for that year. 

Our machine learning model is an ordinary least square linear regression. We are looking for the factors that influence adoptation of solar panels in a community. Variables that we are to include (subject to change) include household income, education, ethnicity, etc., solar irradiance data (whether the amount of sunlight in a region plays a factor in the adaptation in solar panels), region, population. 

Therefore our dependent variable would be the percentage of households with solar panel installations. Independent variables such as household income, education, ethnicity, solar irradiance data, location characteristics (whether it is urban or rural, or in a more northern region) will be tested to see which model has the highest r-squared value, along with the p-values of each variable.The r-square value will assist in validating the effectiveness of the model and whether it will help characterize the individual most likely to install solar panels.

Our hypothesis is that higher-earning households with more years of education will adapt solar panels. We analyze 11 counties that attempt to include most of the major population centers in Michigan, as well as encompass different regions of the state. 
  * Alpena County
  * Calhoun County
  * Genesee County
  * Gogebic County
  * Grand Traverse County
  * Ingham County
  * Kent County
  * Mackinac County
  * Oakland County
  * Washtenaw County
  * Wayne County

We hypothesized that either Oakland County, due to its higher income per household, or Washtenaw County, due to higher education levels, would be the most piviotal factor in solar adapation.

# Resources

**Data:** 

Average Household Income MI - Census Bureau

Homeownership rate in MI - Census Bureau

Renewal Energy Sector in MI - Census Bureau

NREL National Solar Radiation Database 2015 - 2020

DeepSolar by Stanford - https://web.stanford.edu/group/deepsolar/home

# Communication Protocols

Team members collaborated using Zoom for meetings, Git Hub for subitting our work and Slack for all other communications outside of meetings.
