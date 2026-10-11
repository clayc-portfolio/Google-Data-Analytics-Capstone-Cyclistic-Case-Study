# Cleaning and Transforming

## Preparing The Data

Now that we have determined our business task and key question at hand, it's time to take the steps in preparing the data for eventual cleaning and analysis. As mentioned previously, we will be using the divvy_tripdata data to access historical ride information for our analysis. Within the trip data, there are files for each month beginning at April 2020 and ending at August 2025. For this case study, we will be using the ride data from August 2024 through July 2025. Each file has the same naming convention of YYYYMM-divvy-tripdata and includes the same information such as ride id, bike type, start times and stations, end times and stations, and whether the rider is a member or a casual. The data has been made available by Motivate International Inc. under this license.

This is public data that you can use to explore how different customer types are using Cyclistic bikes. But note that data-privacy issues prohibit you from using riders’ personally identifiable information. This means that we won’t be able to connect pass purchases to credit card numbers to determine if casual riders live in the Cyclistic service area or if they have purchased multiple.

During this phase, it's important to recognize where the data is located and how it is organized, allowing you to better understand how to work with the data efficiently. Taking into account the integrity of the data and how the information provided helps answer your question is also important, as this will contribute to a reliable analysis. 

## Processing, Cleaning & Transforming The Data

I have chosen to use excel and SQL to clean my data 

The data is broken down into columns showing each ride's information

- Trip start day and time
- Trip end day and time
- Trip start station
- Trip end station
- Rider type (member or casual)
- Bike type

For the cleaning phase, i created two new columns to calculate the ride duration as well as the day of the week that the ride occurred on. Knowing the day of the week as well as trip during will help drive insights into how casual and members ride differently. 

### Calculating Ride Duration & Day of Ride
Open your spreadsheet and create a column called ride_length. Calculate the length of each ride by subtracting the column started_at from the column ended_at (for example, =D2-C2) and format as HH:MM:SS using Format > Cells > Time > 37:30:55.

Create a column called day_of_week, and calculate the day of the week that each ride started using the WEEKDAY command (for example, =WEEKDAY(C2,1)) in each file. Format as General or as a number with no decimals, noting that 1 = Sunday and 7 = Saturday.








