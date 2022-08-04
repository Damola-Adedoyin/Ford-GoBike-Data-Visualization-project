# Ford GoBike System Data Exploration
## by Damola Adedoyin

> NOTE: view the codes (data wrangling and exploration) in the `Part_I_exploration.ipynb` file and the final presenation (data explanation) in the `Part_II_slide_deck.ipynb` files above.

## Dataset

The [Ford GoBike Dataset](https://github.com/BetaNYC/Bike-Share-Data-Best-Practices/wiki/Bike-Share-Data-Systems) 
originally contained 183412 rows of data and 16 columns. 
Each row represents a ride made in a bike-sharing system around the San Francisco Bay area 
in the United State, for the month of February 2019. The `duration` column shows how long 
it takes a rider to go from one station (`start_station`) to another (`end_station`).

Some cleaning were done to remove rows with missing data and some addition columns were extracted 
from the existing ones to create features to aid better data exploration and analysis. 
Some of the wrangling steps included the following:
- Remove rows with nans
- Extract `weekday`, `month`, and `year` columns from the `start_time` column
- Calculate riders `member_age` columns from the riders' birth year column
- drop irrelevant columns

At the end of the the wrangling, the final dataset that went on to the exploration and visualization 
stages included 174952 rows and 16 columns.


## Summary of Findings

The focus of the exploration was to examine the factors that contributes the most to the stability (and variation)
in ride duration and how these factors affect each other in relation to the target variable (ride duration). 
The modal ride duration range appears to be around rides lasting for about 6mins to about 7 mins, and the median 
duration lies slight higher above this range.  The data appears to be significantly right-skewed, pulling 
the mean of the ride duration to ranging from about 9 to 11mins.

Of all the other features of interest, the features focused on (seeing they had the most obvious effects) 
include the rider start-hour, members type, members gender and members age. The relationship between this
individual features or a combination of then will be presented in the final presentation. 
It was observed that the male gender and the  subscribers looked to have the most stable ride duration as 
compared to other gender categories and customers respectively. Members within a certain age range also showed 
a lot of stability with ride duration and finally, rides around 11am to 4pm showed a fairly stable mean ride duration.


## Key Insights for Presentation

The presentation will show the distribution of the target feature (ride duration) and some of the
other features of interest. It also show some relationships between these features and the 
main/target feature of interest.Histogram, barplots, lineplots, etc. are used where applicable and 
color encoding (with labeled legends) are used appropriately to distinguish between different variables.
