# LTFS-Data-Science-FinHack-2
Forecast number of applications received by LTFS.

# Problem statement

LTFS receives a lot of requests for its various finance offerings that include housing loan, two-wheeler loan, real estate financing and micro loans. The number of applications received is something that varies a lot with season. Going through these applications is a manual process and is tedious. Accurately forecasting the number of cases received can help with resource and manpower management resulting into quick response on applications and more efficient processing.
You have been appointed with the task of forecasting daily cases for next 3 months for 2 different business segments at the country level keeping in consideration the following major Indian festivals (inclusive but not exhaustive list): Diwali, Dussehra, Ganesh Chaturthi, Navratri, Holi etc. (You are free to use any publicly available open source external datasets). Some other examples could be:

*	Weather

*	Macroeconomic variables

 Note that the external dataset must belong to a reliable source.

[Data Source](https://datahack.analyticsvidhya.com/contest/ltfs-data-science-finhack-2-an-online-hackathon/)

# Data Dictionary

The train data has been provided in the following way:

*	For business segment 1, historical data has been made available at branch ID level
*	For business segment 2, historical data has been made available at State level.
 
# Train File

|Variable|	Definition|
|---------|------------|
|application_date	|Date of application|
|segment	|Business Segment (1/2)|
|branch_id|	Anonymised id for branch at which application was received|
|state	|State in which application was received (Karnataka, MP etc.)|
|zone|	Zone of state in which application was received (Central, East etc.)|
|case_count	|(Target) Number of cases/applications received|
 
# Test File

Forecasting needs to be done at country level for the dates provided in test set for each segment.

|Variable	|Definition|
|---------|-----------|
|id	|Unique id for each sample in test set|
|application_date|	Date of application|
|segment|	Business Segment (1/2)|
 
# Sample Submission

This file contains the exact submission format for the forecasts. Please submit csv file only.

|Variable|	Definition|
|---------|------------|
|id	|Unique id for each sample in test set|
|application_date	|Date of application|
|segment|	Business Segment (1/2)|
|case_count	|(Target) Predicted values for test set|
 
Note that you can only make 5 submissions per day

# Evaluation

# Evaluation Metric

The evaluation metric for scoring the forecasts is MAPE (Mean Absolute Percentage Error) 

The Final score is calculated using MAPE for both the segments using the formula:

Final = 0.5 x MAPE(segment-1) + 0.5 X MAPE(segment-2)
 
# Public and Private Split

Test data is further divided into Public (1st Month) and Private (Next 2 months)

*	Your initial responses will be checked and scored on the Public data.
*	The final rankings would be based on your private score which will be published once the competition is over.

## Public score: 30.01     Rank: 298

## Private score: 47.87    Rank: 349

## Winner's score: 10.00/19.8

