# Analysis of Temperatures in June and December 
## Overview of Analysis
This project was scoped to review the temperatures measured in the months of June and December, with the intent to have information to plan for the opening of a surf and ice cream shop in Hawaii.  

Source information was provided in a SQLite database to be queried against.  This data was queried using SQLite and SQLAlchemy and imported into a Pandas DataFrame for analysis.  

## Data Scrubbing 
Once the SQLite database was stored locally, it was queried to access the tables and the data they contained.  The data points available are the US Weather Station, the date of the measurement, any precipitation totals, and the temperature observation for that date.    SQLAlchemy was used to extract the date and temperature observations for the study  months (June and December) for years 2010 through 2017.  This information was then converted to a Pandas DataFrame and summary statistics for the data were calculated which will be compared later in this analysis. 

## Results Review
Subjective result: June OR December would be an optimal time to visit Hawaii.  
 
### June 
|Measure|Value|
|---|---|
|Count|1700|
|Mean|74.94|
|STD|3.25|
|Min|64.0|
|25%|73.0|
|50%|75.0|
|75%|77.0|
|Max|85.0|

### December 
|Measure|Value|
|---|---|
|Count|1517|
|Mean|71.04|
|STD|3.74|
|Min|56.0|
|25%|69.0|
|50%|71.0|
|75%|74.0|
|Max|83.0|

### Comparisons 
Data Set 
: The June dataset contains 1700 records.
: The December dataset contains 1517 records. 

Minimum Temperatures
: The minimum temperature in June is 64.0
: The minimum temperature in December is 56.0 

Maximum Temperatures
: The maximum temperature in June is 85.0 
: The maximum temperature in December is 83.0 

Average Temperatures
: The mean temperature in June is 74.94
: The mean temperature in December is 71.04

Key Differences
: There is an 8 degree difference between the minimum temperatures in June (64) and December (56)
: There is a 2 degree difference between the maximum temperature in June (85) and December (83)
: There is a 3.9 degree difference between the mean temperature in June (74.94) and (71.94) 

## Summary 
### High Level Analysis 
For the most part, there are not dramatic differences between the temperatures in June and December.  The largest difference is in the minimum temperatures (8 degrees).  Because of these fairly stable temperature differences, it can be assumed that business would be stable throughout the year, providing customer traffic to support a new business.  

### Suggested Additional Data Points 
In addition to temperatures, it is recommended to include precipitation analysis between June and December.  This has been included in the data sets and queries that are included in this project.  

Out of the total number of records for June, (1574) there were 927 days where there was some precipitation. This is approximately 58.9% of dates in June.  In comparison, there were 895 days in December that had precipitation (total number of records - 1405) This is approximately 63.7% of dates in December with some level of precipitation.    While this gives an approximate indication that December is the rainy season in Hawaii, additional data cleaning should be done to remove records that do not have both a temperature and precipitation reading prior to doing these calcuations.  This will provide a more accurate picture of weather patterns. 

### Suggested Additional Considerations 
This information will provide a foundation to business decisions that should be made for the anticipated business creation, however there are some additional data points that should be considered.  These are outside of the scope of this project and are not included in the data that was provided for analysis, but may be helpful for business planning. 

Travel Seasons 
: There are travel seasons that would drive additional business to the SurfsUp shop.  These seasons could include holidays, school breaks, spring break, summer vacations
International Travel 
: Travel from other countries would also drive business to the shop.  These travel schedules are often quite different from typical domestic travel.  Again, holidays, school breaks, spring breaks and other vacations should be considered.  (These could possibly be polar opposites to domestic travel due to geographic differences)
Wedding Season
: Hawaii is a location that is often favored for honeymoons and anniversaries.  Trends in this area should also be considered and analyzed for planning. 


