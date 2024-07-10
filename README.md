# Cyclistic Analysis

Sathish |
Data Analyst |
20/09/2023 |
sathishgudri@gmail.com |
Bangalore, India |

# About:
Cyclistic is a successful bike sharing company which was launched on 2016. Since then, the program has grown to a fleet of 5824 bicycles that are geo-tracked and locked into a network of 692 stations across Chicago.The bikes can be unlocked from one station and returned to any other station in the system anytime.

Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the ﬂexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.

# Me & My Team
I am a Junior Data Analyst in the Marketing Analyst Team of the company. The director of the team believes that company’s future success depends on maximizing the number of annual memberships.

Rather than creating a marketing campaign that targets all-new customers, the director believes there is a very good chance to convert casual riders into members, as they have already aware of the Cyclistic Program and have chosen Cyclistic for their mobility needs. Therefore, the team is focused to design marketing strategies aimed at converting casual riders into members of the company.

# Objective
Our primary goal is to convert casual riders into loyal members of the company. In pursuit of this objective, my task was to understand the differences in riding preferences and behaviours exhibited by casual and member riders and to give top three recommendations based on the analysis.

# About Dataset
The dataset covers the time period from June 22 to July 23. The data comes from the company's cloud.

 A limitation of the dataset is its lack of information regarding the distance covered in each ride, which I believe is essential information that should have been incorporated.

 # Workings
 I started my work by downloading the zip files from the given website link and unzipped the files. There were 12 files containing the data relating to 12 months. The files were in CSV format. I first opened some of the random files to have a glance and understand the dataset better. It was a big dataset and I understood it was hard to work using MS excel. I decided to go with SQL and loaded all those data into Cyclistic Database that I created in PostgreSQL server.

 

1)       Data cleaning:

* Merged all data into single table in SQL.

* Checked for the duplicate values in the dataset to exclude them from analysis. However, the data looked already cleaned as there were 
  no duplicate records.

* Data contained some non-useful information about the rides, like latitude and longitude of the trip’s start and end destination, which 
  in my opinion was unnecessary for my analysis. Hence such non-relevant information were excluded from the analysis.

* There were some empty spots in the columns that had names and IDs for the starting and ending stations of the trips. Since there were 
  so many missing values, I decided not to use these columns to make sure my results were accurate.

 

2)       Manipulation of Data:

* Calculated the Weekday of the trip starting date to identify the favourable days of riders.

* Calculated the duration of each trips to get insight about the riding duration.

* Created a column to show the season to understand the seasonal behaviour of the customers.

* Extracted month from the date to understand the monthly ride trend.

* Calculated the Time of the Day (Morning, Afternoon etc.) to identify the customer preferences.

 * Extracted the starting time from the ‘started at’ column to identify the most crowded hours.

 

3)       Key Findings:

**Usage Patterns Over the Day:**

* A notable convergence exists between the usage patterns of casual and member riders based on the time of day.

* Both rider categories show a preference for riding during the afternoon and the morning hours.

 

**Monthly and Seasonal Riding Trends:**

 * The peak riding period aligns with the summer season, followed closely by the fall season.

* Winter witnesses the lowest ridership, both among members and casuals.

* During winter, casual rides comprise only 2.19% of the total rides, while in summer, this figure escalates to 19.46%, reflecting  a substantial 17.27% shift.

* Member rides during winter account for 7.46%, compared to the summer's 21.35%, signifying a significant 13.89% change.


**Riding Frequency on Weekdays:**

* Casual riders exhibit a preference for weekends, especially Saturdays. In contrast, members prefer weekdays, with  Wednesdays 
  registering their highest ridership.

* Mondays see the fewest casual rides, whereas for members, it's Sundays that record the lowest ridership.

 

**Preferred Rideable Types by Rider Category:**

* Electric bikes hold the highest appeal among both members and casuals, closely followed by classic bikes. Docked bikes rank as the 
  least preferred option. Interestingly, members entirely avoided docked bikes during the dataset period.

 

**Ride Duration in Minutes:**

* The majority of rides taken by both rider groups last approximately 4 to 5 minutes.

* On average, member rides endure around 12 minutes, while casual rides extend to about 20 minutes. This underscores the inclination of 
  casual riders towards longer rides.

 

**Time Distribution of Total Rides:**

* Among members, 5 PM emerges as the peak riding time, closely trailed by 8 AM. This strongly suggests that members primarily use the 
  bikes for commuting purposes.

* Casual riders exhibit a consistent uptick in ride frequency from 4 AM until 5 PM. This indicates that casual riders often use the 
  bikes for leisurely trips.

 

4)       Visualization :

Created visually appealing graphs and charts to showcase the above analysis through visualization.

# Top Three Recommendations
**Summer Promotion Campaigns:**

As summer records the most number of rides, create special summer membership packages that encourage the casual riders to become members during this peak riding period.


**Weekend exclusive offers:**

Recognizing the weekend preference of casual riders, consider designing weekend exclusive offers that encourage casual riders to experience the benefits of membership during their preferred time.


**Commute Benefits:**

Focus on promoting the convenience and cost-effectiveness of annual membership for daily commuting. Highlight the busiest time for members (5 PM) and emphasize how having a membership can make their daily commute more efficient and hassle-free.

