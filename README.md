# V2_Cipparone_Niva_OCallaghan_EDA_Finalproject
Duke Univeristy EDA 872

At the beginning of the project we had utilized another repository but had issue committing files to github. After discussions with Professor John Fay it was decided to create a new repository. The link the to old repository is below. 
https://github.com/arielocallaghan/Cipparone_Niva_OCallaghan_EDA_Finalproject

## Summary

<This repository was created for an Environmental Data Analytics Class at Duke University Nicholas School of the Environment. This repository contains information on Pennsylvania coal production, Census data, water quality, and community health rankings. This project was started in late November 2022 and will be completed by December 14, 2022. The goal of this project is to understand the impact coal production has on community health indications. This analysis focus only on Pennsylvania as this state is forth largest coal producing state in the Nation. A multivariate regression and time series analysis will be utilized as the primary form of analysis.The analysis has been completed at the county scale as that was the granularity available for the datasets we wanted to use.>


## Investigators

<Contributors to this repository include Hugh Cipparone, Katryna Niva and Ariel O'Callaghan all students at Duke University>


## Keywords

<Pennsylvania, Coal production, community health>

## Database Information

<Coal Production data: Raw data was collected from the U.S. Energy Information Administration (EIA).The EIA is the statistical and analytical agency within the U.S. Department of Energy. Their purpose is to collect, analyze and disseminate information on energy information. EIA is the governments primary source for energy information and data. The data utilized was from the coal data webpage from their production tab. The entire time frame of data available has been utilized for this report. This data was first accessed on November 22, 2022. 

Link:https://www.eia.gov/coal/data.php (Production tab)

water Quality: Water Quality Portal: This portal integrates water quality data from the United States Geological Survey (USGS) and Environmental Protection Agency (EPA), and over 400 state, federal, and local agencies. Water quality information was downloaded for Pennsylvania, with data spanning from 1991 -2011. This data was accessed on November 27, 2022.

Link: https://www.waterqualitydata.us/

Census Data: This data set is the American Community Survey (ACS) data set and is part of the U.S. Census. The ACS provides survey information on a yearly basis about our nation and its people. It is the pmary data source of the U.S. Census for detailed information on population and housing information. This data was accessed on November 26, 2022. 

link:https://www.census.gov/programs-surveys/acs/data.html

Community Heath data: This data was collected and downloaded from County Health Rankings and Roadmaps. This is a program out of the University of Wisconsin Population Health Institute. This program developed a community health ranking model and their indicators were utilzed for this analysis. Data was download for Pennsylvania from 2010-2020. This data was accessed on November 28, 2022. 

Link: https://www.countyhealthrankings.org/explore-health-rankings


## Folder structure, file formats, and naming conventions 

<Folders:
Raw Data: This is the data imported as a .csv with out any wrangling or manipulation. All raw data sets utilized in analysis for this project are located here. 

Processed Data: This folder contains data that has been wrangled to include the information needed for further analysis. Additionally it contains combined data sets of individual years of each database download combined into once csv file. The combine.csv file is a combination of all the individual data sets after they have been wrangled into one complete file. This file contains all the information needed for analysis conducted during this project. Some additional dataframes were made with subsets of data contained in the combined.csv to simply further analysis.  

Data Wrangled: This folder contains the rmd files utilized to wrangle and manipulate the individual data sets. Additionally, it contains code for creating visualizations, summary statistics and plots.

Data Analysis: This folder contains rmd files used to analyze our complete data set.

Report: This folder contains the rmd file of our report that was written and prepared for the class project. Additionally it contains some reference documents on the project requirements and some rmd cheat sheets for quick reference. 

The files were named off of the type of data that that is analyzed:   
-Health files are for the community health indicator  
-acs files are for the census data  
-coal files are for the coal production numbers. This also includes some water quality data. 
-water quality data: Water quality data from the portal described above. 

Other naming conventions include:  
visualizations: These rmd files were utilized to create ggplots, graphs and tables utilized in the report.    
cleaning: Refers to rmd files utilized to do additional wrangling for analysis   
df_combine: This is the rmd file utilized to take all of the individual data frames and create one df for future analysis. The output of this rmd file is the combined.csv.   

The analysis rmd file names show the type of analysis that is conducted. >
MLR: Multiple linear Regression
Time Series: Time series analysis:
Spatial: Spatial representation of the community health indicators. The community health data is displayed visualizing. The county cartographic boundary shapfiles developed by the U.S. Census were downloaded here https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html

## Metadata

complete.csv This file contains all of the individual data sets combined into one complete data frame. The only information not in this complete.csv is the water quality information described separately below. 

**Columns Names Below:**
<The csv file is organized so that all Counties in Pennsylvania are rows and each row contains the following columns. Some data sets have varying date ranges so some columns show NA when there is no data available. 

--complete.csv--

**County:** All Counties in Pennsylvania   class:"factor"      
**Year** Year Class: "Date"    
**totpop:** Total population by County  Class:"Numeric"    
**medage:** Median Age  Class:  "Numeric"    
**totpoprace:** population of non white people Class: "Numeric"  
**totpopwhite:** Population of white people	Class:"Numeric"  
**totpopeduc:** population of educated people  Class: "Numeric"  
**bachdegree:** Population of people with bachelor degrees  Class:"Numeric"	      
**medincome:** Median Income 	  Class:"Numeric"   
**perc.white:** Percentage of White people	 Class:"Numeric"      
**perc.bachdegree:** Percentage of bachelor degrees Class:"Numeric"         
**year:** Date information for each indicator 	  Class:"Numeric"       
**coal.prod.by.year:** Coal production by year (Tons)	  Class:"Numeric"       
**year.peak.prod:** Year of peak coal Production (Tons)  Class:"Numeric"      
**sum.coal.prod:** Sum of total coal production  	(Tons)  Class:"Numeric"       
**Health.Outcomes.Z.Score:** This is a z score. Health outcomes looks at length of life and quality of life. Length of life looks at premature death and life expectancy and quality of life measures of low birth weight and those who rated their physical and mental health as poor. This outcomes puts a 50% weight on both Quality of Life and Length of life.  Class: "numeric"    
**Health.Outcomes.Rank:** The rank of health outcomes with 1 being the healthiest Class:"numeric"   
**Health.Factors.Z.Score:** Z score. Health factors includes health behaviors, clinic care, social and economic factors and physical environment.       
**Health.Factors.Rank:**  Rank of Counties with 1 being the healthiest  Class:"numeric"    

--Water Quality Data set--    
**Date:** The date the sample was collected Class:"Date"  
**Location** The location of the sample Class:"Character"  
**Latitude** The coordinates of the sample Class:"Numeric"  
**Longitude** The coordinates of the sample "Class:Numeric"	  
**County.Code**	Number as a reference to the county code class"Character"  
**Contaminant** The element that is being sampled ie. iron class"Character"  
**State**	The type analysis run on the sample. i.e. in dissolved form Class:"Character"  
**Measure** The sample result Class:"Numeric"  
**Units** The units of that sample ie. mg/L class:"Numeric"  
>


## Scripts and code

**Data Analysis Folder**    
<The MLR.rmd is a code to conduct the multiple liner regression analysis. This code also contains correlation plots between each variable of interest. This code look a a few specific counties of coal production and health indicators.  

The Timeseries.rmd code is to examine the relationship between health outcomes and coal production for 2010-2010. 

**Data Wrangling**   
The ACSDataCleaning.rmd is the file utilized to clean the ACS data to get only the parameters of interest. 

The ACSImportraw.rmd is the import file each of the individual raw datasets utilized from the census.

TheACSVisualization.rmd this file is utilized to prepare visualizations and ggplots.

The df_combine_HC.rmd is the file utilized to create the master dataframe called complete.csv This takes all of the individual datframes ie. health, coal and puts them together. 

The HC_CoalWrangle.rmd is file utilized to calculate total production by county.

The healthdata.rmd is the file utilized to import and wrange the community health indicators.

The healthtable.rmd is the file utilized for the knable function to make the summary statistics table.

The healthvisualizations.rmd is the file utilized to explore the health data set and prepare visualizations utilizing ggplot. 

The KN.Coal.rmd is hte file utilized to import, wrangle and prepare visualizations for the coal production data and water quality parameters.

The MLR_Wrange.rmd is the file utilized to wrangle the data to prepare it for the multiple linear regression. 

The spatial.rmd utilized the community health indicators to represent them by county on a map.>


## Quality assurance/quality control

The team has worked together to check each others work. The complete data frames and other wrangling procedures have been discussed and QA/QC'ed by one other team member. Additionally, we have looked at each others analysis and outputs and helped each other with results interpretation. 
