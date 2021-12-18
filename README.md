# Kickstarting with Excel

## Overview of Project

Provide a report that can provide summary insights to results per country of kickstarts campaigns from 2009 to 2017. 

### Purpose

The goal of this project is to provide summary level information of how campaigns fared based on their launch date and funding goals outcomes. 
The attached report can provide the necessary information so Ms. Louise can analyze the results of her play Fever vs other previous campaigns. 
The aim is to accomplish that more campaigns in the future can be achieve their goals in the shortest time possible.   

## Analysis and Challenges

### Analysis
This project aims to provide summary-level information of how campaigns fared based on their launch date and funding goals outcomes. 
The attached report can provide the information required so Ms. Louise can analyze the results of her play Fever vs. other previous campaigns. 
The aim is to accomplish that more campaigns in the future can achieve their goals in the shortest time possible.

### Challenges
Some challenges will be present based on the original request as with any other data set. 
The challenges presented in the project were two types Incomplete or missing data; please see section Challenges and how it was solved.



### Analysis of Outcomes Based on Launch Date

Launch dates provides a view of success and failures based on the seasonality.  

### Analysis of Outcomes Based on Goals

Based on Goals provides a view of success and failures based on the goal threshold.  

### Challenges and Difficulties Encountered

Incomplete or missing data: 

	-Percentage Fund missing:   This issue was solved by calculating per kickstart campaign using the formula 
	 = (Pledged $ / goal $) * 100, rounded to the two using round function in excel. 
 
	-Average donation missing    Added to the data set by calculating per each kickstart campaign using the formula 
	 = (Pledged $ / backers count)
 
	-Parent Category and Subcategory classification joined: Parent category and subcategory data separated and added 
	 to the data set via text to column feature in excel using the ( / ) as the delimiter. 
 
	-Date created: original data set provide the launched kickstart date using the UNIX format date system. 
	 The conversation to Month/Day/Year or MM/DD/YYYY format was achieved by the following formula 
	 = ((( UNIX Date reference Cell / 60  )/ 60 )/ 24 ) + DATE(1970,1,1). 
 
	-Years missing: leveraging the date created cell, the function = Year ( Date Created cell ) 
	 was applied to extract the start year of the kickstart. 
 
	-Goal Range missing sorted the goals in descending order, then filtering the data by the necessary ranges 
	 and flag manually the goal corresponding bucket into a new column named “Goal range.”   


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

	- The best months to have a successful campaign is from March to June. 
	- The most successful kickstarts are plays, rock, documentaries, and classical music. 


- What can you conclude about the Outcomes based on Goals?

	- Goals less than $5,000.00 are the most successful with a success rate of 73% and over. 
	- Goals between $5,000 and $25,000 have an average success rate 51%. 
	- Goals over $25,000 have an average success rate of 32%. 

- What are some limitations of this dataset?

As with any dataset, some data points are not part of the original data. 
Thus, we need to build the data points required to respond the questions. 

- What are some other possible tables and/or graphs that we could create?

	-Table: Subcategories and Goals
	-Table: Years and Outcome. 


