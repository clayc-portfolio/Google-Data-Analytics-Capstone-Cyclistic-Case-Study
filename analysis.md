# Analysis

## Excel was used for additional analysis to gain further insights about the dataset. 

### Excel Analysis

I wanted to determine the mean of each ride duration, the maximum ride length, and the day of the week that is most popular 

Using the newly created columns of ride length and day of the week, we calculated the following :

- Mean of ride Length:	00:22:07
- Max ride length:	15:30:24
- Mode day of The week: 3

We also grouped the data using a pivot table 

<img width="380" height="392" alt="image" src="https://github.com/user-attachments/assets/76164ac0-d19a-43af-bd6a-e8ee81a62eec" />

### SQL Analysis

For more information on SQL queries, navigate to analysis.sql

-- looking for duplicate records
-- looking for null values 
-- Making sure theres only two types of members
-- Looking for any errors/mispelling/inconsistencies in rideable types
-- count all total rows = 5860776
-- count all rows with empty strings. total rows with missing values = 1193477
-- delete all rows with empty strings
-- total rows after removing empty strings = 4667299 
-- Add new column for day of the week, ride length 
-- convert date time to weekday
-- set duration of each trip in seconds
-- check for duration with negative values 
-- count rows with less than 60 seconds = 64220 rows
-- delete rows with less than 60 seconds
