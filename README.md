# V2_Cipparone_Niva_OCallaghan_EDA_Finalproject
Duke Univeristy EDA 872

At the beginning of the project we had utilized another repository but had issue committing files to github. After discussions with Professor John Fay it was decided to create a new repository. The link the to old repository is below. 
https://github.com/arielocallaghan/Cipparone_Niva_OCallaghan_EDA_Finalproject

## Summary

<This repository was created for an Environmental Data Analytics Class at Duke University Nicholas School of the Environment. This repository contains information on Pennsylvania coal production, Census data, water quality, and community health rankings. This project was started in late November 2022 and will be completed by December 14, 2022. The goal of this project is to understand the impact coal production has on community health indications. This analysis focus only on Pennsylvania as this state is forth largest coal producing state in the Nation. A multivariate regression and time series analysis will be utilized as the primary form of analysis. For this project a time series analysis will also be utilized.>


## Investigators

<Contributors to this repository include Hugh Cipparone, Katryna Niva and Ariel O'Callaghan all students at Duke University>


## Keywords

<Pennsylvania, Coal production, community health>

## Database Information

<Coal Production data: Raw data was collected from the U.S. Energy Information Administration (EIA) coal production tab. This data was first accessed on November 22, 2022. 

Link:https://www.eia.gov/coal/data.php (Production tab)

water Quality: Water Quality Portal: This portal integrates water quality data from the United States Geological Survey (USGS) and Environmental Protection Agency (EPA), and over state, federal, and local agencies. Water quality information was downloaded for Pennsylvania, with data spanning from 1991 -2011. This data was accessed on November 27, 2022.

Link: https://www.waterqualitydata.us/

Census Data: This data set is the American Community Survey (ACS) data set and is part of the U.S. Census. The ACS provides survey information on a yearly basis about our nation and its people. This data was accessed on November 26, 2022. 

link:https://www.census.gov/programs-surveys/acs/data.html

Community Heath data: This data was collected and downloaded from County Health Rankings and Roadmaps. Data was download for Pennsylvania from 2010-2020. This data was accessed on November 28, 2022. 

Link: https://www.countyhealthrankings.org/explore-health-rankings


## Folder structure, file formats, and naming conventions 

<Folders:
Raw Data: This is the data imported as a .csv with out any wrangling or manipulation. All raw data sets utilized in analysis for this project are located here. 

Processed Data: This folder contains data that has been wrangled to include the information needed for further analysis. Additionally it contains combined data sets of individual years of each database download combined into once csv file. The combine.csv file is a combination of all the individual data sets after they have been wrangled into one complete file. This file contains all the information needed for analysis conducted during this project. Some additional dataframes were made with subsets of data contained in the combined.csv to simply further analysis.  

Data Wrangled: This folder contains the rmd files utilized to wrangle and manipulate the individual data sets. Additionally it contains code for creating visualizations, summary statistics and plots.

Data Analysis: This folder contains rmd files used to analyze our complete data set.

Report: This folder contains the rmd file of our report that was written and prepared for the class project. Additionally it contains some reference documents on the project requirements and some rmd cheat sheets for quick reference. 

The files were named off of the type of data that that is analyzed:   
-Health files are for the community health indicator  
-acs files are for the census data  
-coal files are for the coal production numbers. This also includes some water quality data. 

Other naming conventions include:
visualizations: These rmd files were utilized to create ggplots, graphs and tables utilized in the report.
cleaning: Refers to rmd files utilized to do additional wrangling for analysis 
df_combine: This is the rmd file utilized to take all of the individual data frames and create one df for future analysis. The output of this rmd file is the combined.csv. 

The analysis rmd file names show the type of analysis that is conducted. >
MLR: Multi linear Regression
Time Series: Time series analysis:
Spatial: Spatial repersentation of the community health indicators. 

## Metadata

complete.csv This file contains all of the indivudal data sets combined into one complete data frame. 

**Columns Names Below:**
<The csv file is organized so that all Counties in Pennsylvania are rows and each row contains the following columns. Some data sets have varying date ranges so some columns show NA when there is no data available. 

**County:** All Counties in Pennsylvania   class:"factor"    
**Year** Year Class: "Date"  
**totpop:** Total population by County  Class:"Numeric"  
**medage:** Median Age  Class:  "Numeric"  
**totpoprace:** xxxx Class: "Numeric"
**totpopwhite:** Population of white people	Class:"Numeric"
**totpopeduc:**   XXXX  Class: "Numeric"
**bachdegree:** Number of people with bachelor degrees  Class:"Numeric"	    
**medincome:** Median Income 	  Class:"Numeric" 
**perc.white:** Percentage of White people	    Class:"Numeric"    
**perc.bachdegree:** Percentage of bachelor degrees Class:"Numeric"     
**year:** Date information for each indicator 	  Class:"Numeric"     
**coal.prod.by.year:** Coal production by year (Tons)	  Class:"Numeric"     
**year.peak.prod:** Year of peak coal Production (Tons)  Class:"Numeric"    
**sum.coal.prod:** Sum of total coal production  	(Tons)  Class:"Numeric"     
**Health.Outcomes.Z.Score:** This is a z score. Health outcomes looks at length of life and quality of life. Length of life looks at premature death and life expectancy and quality of life measures of low birth weight and those who rated their physical and mental health as poor. This outcomes puts a 50% weight on both Quality of Life and Length of life.  Class: "numeric"  
**Health.Outcomes.Rank:** The rank of health outcomes with 1 being the healthiest Class:"numeric" 
**Health.Factors.Z.Score:** Z score. Health factors includes health behaviors, clinic care, social and economic factors and physical environment.     
**Health.Factors.Rank:**  Rank of Counties with 1 being the healthiest  Class:"numeric"  

>

<For each data file in the repository, describe the data contained in each column. Include the column name, a description of the information, the class of data, and any units associated with the data. Create a list or table for each data file.> 

## Scripts and code

<list any software scripts/code contained in the repository and a description of their purpose.>

## Quality assurance/quality control

The team has worked together to check each others others data and analysis. The complete data set was verified accurate but all team members. We have QA/QC each others analysis and results. 
