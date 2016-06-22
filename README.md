# DoingDataScience_CaseStudy
__________________________

###Claire Chu
###Doing Data Science 6306
###Case Study Assignment

---------------------------
#####Please access the main project file through "CChuDDS_CaseStudy.Rmd"
#####Please access the Raw Data through the Analysis/Data directory
#####Please access the code .txt file and graph output through the Analysis directory
-----------------------------
#I. INTRODUCTION TO THE PROBLEM
#####We will explore two datasets; one that details the GDP rankings worldwide and another which details various income statistics for countries around the world. Both datasets will be downloaded raw from http://data.worldbank.org/data-catalog and munged with the code that follows. Once cleaned, we will focus our analysis on the GDP rankings and Income groupings for the top 190 countries worldwide.
--------------------------
#II. DOWNLOAD THE FILES
#####Download the data from the provided links.
--------------------------
#III. READ THE FILES
#####Work through reading in the GDP and EDUC dataset.
--------------------------
#IV. CLEAN THE DATASETS
#####Clean up the GDP and EDUC dataset.
--------------------------
#V. MERGE THE DATASETS
#####Merge the datasets together to prepare data for analysis.
---------------------------
#VI. ANALYZE THE DATA
#####1	Match the data based on the country shortcode. How many of the IDs match? 
#####2	Sort the data frame in ascending order by GDP rank. What is the 13th country in the resulting data frame?
#####3	What are the average GDP rankings for the "High income: OECD" and "High income: nonOECD" groups? 
#####4	Plot the GDP for all of the countries. Use ggplot2 to color your plot by Income Group.
#####5	How many countries are Lower middle income but among the 38 nations with highest GDP?
---------------------------
#VII. CONCLUSION
#####Based on the analysis, we can see that the top ranking GDP countries mainly consist of countries of the “High Income OECD” group. Why is this? A quick search of “OECD Countries Meaning” displays the following definition.
#####“The Organisation for Economic Co-operation and Development (OECD) is an international economic organisation of 34 countries, founded in 1961 to stimulate economic progress and world trade.” -https://en.wikipedia.org/wiki/Organisation_for_Economic_Co-operation_and_Development
#####This would make sense then, that the top countries reporting their GDP data to this entity would be the countries that are actively trying to stimulate economic progress and world trade. We can see from the data that 24 of the 34 countries exist in the first quantile of the GDP Rankings.
#####From our analysis, we can also see that there are only a few countries in the top ranked GDPs that are also classified as “low income”. In fact, the first “low income” country “Bangladesh” does not occur until the second quantile.
#####Further research of the data reveals that…
#####“As of 1 July 2014, low-income economies are defined as those with a GNI per capita, calculated using the World Bank Atlas method, of $1,045 or less in 2013; middle-income economies are those with a GNI per capita of more than $1,045 but less than $12,746; high-income economies are those with a GNI per capita of $12,746 or more. Lower-middle-income and upper-middle-income economies are separated at a GNI per capita of $4,125. Note that low- and middle-income economies are sometimes referred to as developing economies.” -http://data.worldbank.org/news/2015-country-classifications
#####This is consistent with our findings that countries with a “low income” classification (e.g. Bangladesh ranked at 59th) would rank lower than most countries with a “high income: OECD” classification in GDP (e.g. United States ranked in 1st).
