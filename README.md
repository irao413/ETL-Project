# ETL_Francisco_Ian_Scotty

Submission date: 30 April 2020
Team Members: Scotty, Ian and Francisco

Overview
Our group decided to tackle the logistics industry. We will perform an ETL process forMaxianet’s international operations. Maxianet helps brands create new revenue in foreignmarkets. We distribute various consumer goods to countries in North America, Central America,South America, Europe, Africa and Asia. Our focus is on volume and market leadership. For this project we will narrow our scope to Ecuador and the USA. The ETL will yield a centralized data frame from which the company will be able to query much more effectively.


EXTRACT 

The data used for this project came from two sources: United States Craft Beer Brand Data and Mexico Craft Beer Brand Data. The data extraction consisted of two main scrapping processes. The first scaping allowed us to extract all the Beer IDs for each country. These IDs allowed us to open more detailed info about each location within each country. The second scraping extracted the actual data we wanted to use.

We have two scraping tables that can be viewed as PNGs in the repository.



TRANSFORM
The first transformation we performed after exporting the data from the second scraping was clearing out all NA values. Since there was a very large number of variables (beer types) most shops did not offer very single beer, by consequence, most rows had at least one NA value. For this reason we could not all rows containing NA values, we would have been left out with virtually no data. We decided that the most convenient path was to make all NA values equal to 0.

The second transformation we performed was to join both tables. Each table contains data from a specific country, USA and Mexico.

{data normalization}


LOAD
	
Mongo DB has been chosen as the final database.
