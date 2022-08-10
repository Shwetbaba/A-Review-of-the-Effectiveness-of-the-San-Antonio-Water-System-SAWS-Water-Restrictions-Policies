# A Review of the Effectiveness of the San Antonio Water System (SAWS) Water Restrictions Policies
## Overview
The topic was chosen as a starter project for the contributors to apply the skills they have attained in their Data Analytics Bootcamp. This is the first group project of the bootcamp, and as such- the scope will be very limited. Many contributors are new to either data analytics or math, or both. The limitation of the scope enables the contributors to apply the knowledge learned without the additional anxiety of needing to apply things they have not yet learned. 
The group of contributors are located within the San Antonio area, and-like many in the area-find the city appears to be under water restrictions daily. With this in mind, they decided to investigate the determining factors driving these restrictions. Were the water restrictions helping to replenish the well, keep it at a steady level, or was the water level decreasing regardless of these restrictions.
## Variable Determination
Dependent variable will be the Water Levels of the J17 well over a period of 6 years (2016-2022)
Drought information- when the drought category is D1 or higher, does the J17WL well water level increase, decrease or remain constant -to determine if water restrictions are effective?
Quantitative effect of temperature on the water levels- this is to say perhaps SAWS could implement something more strict to prevent water level dropping during high temps?
Quantitative effect of humidity on the water levels and drought levels-->this is for fun to see if there are +/- correlations between drought or water levels and humidity -->maybe extrapolate a finding that when humidity is high and we are in drought- that water restrictions are not as necessary as when humidity is low?
## Findings
The null hypothesis- that the SAWS is maintaining the water levels by implementing water restrictions- was determined to be false.
Several variables were researched to determine if a relationship existed between the water levels and the variables, thus causing the water levels to drop or rise.
* Temperature: While temperature will cause water to evaporate over time, the temperature pattern for the years specified (2016-2022) displayed a normal seasonal pattern. No major outliers to explore
* Humidity: Showed no correlation with the rise or fall in the water levels of the J17 well. No further testing done.
* Precipitation: Slight correlation noted. More noteable significance was the 8.4 ft drop in water level occurring in 2020, the water level never again reached the 2016-2019 average levels.
* J17 Well levels: used to determine the effectiveness of the SAWS water restriction policy. Found to be dropping steadily, regardless of water restrictions implemented to mitigate this effect.
See accompanying notebook and powerpoint for visuals
## MetaData
* [Weather Historical Data](https://www.wunderground.com)


|Column Name           | Description                                                                                                                 | Data Type     |
|----------------------|:----------------------------------------------------------------------------------------------------------------------------|--------------:|
|Year                  | Year                                                                                                                        | YYYY Format   |
|Month                 | Month                                                                                                                       | MON Format    |
|Day                   | Day of the month                                                                                                            | Integer Format|
|Temp Max              | Maximum temperature recorded for the day                                                                                    |Standard Number|
|Temp Avg              | Average temperature of all temperatures recorded for the day                                                                |Standard Number|
|Temp Min              | Minimum temperature recorded for the day                                                                                    |Standard Number|
|Humidity Max          | Maxiumum level of humidity recorded for the day                                                                             |Standard Number|
|Humidity Avg          | Average of all humidity levels for the day                                                                                  |Standard Number|
|Humidity Min          | Minimum humidity level recorded for the day                                                                                 |Standard Number|
|Precipitation Total   | Total precipation recorded for the day                                                                                      |Standard Number|

* [J17WL Well Historical Data](https://www.edwardsaquifer.org/science-maps/aquifer-data/historical-data/)

|Column Name           | Description                                                                                                                 | Data Type     |
|----------------------|:----------------------------------------------------------------------------------------------------------------------------|--------------:|
|Site                  | J17WL is the naming convention to describe Bexar County Well                                                                | Text Format   |
|DailyHighDate         | Describes the date the measurement of the water level was taken                                                             | MM/DD/YYY     |
|WaterLevelElevation   | The highest observance (in feet above sea level) recorded for a given date                                                  |Standard Number|

* [Drought Conditions](https://droughtmonitor.unl.edu/DmData/DataDownload.aspx)

|Column Name           | Description                                                                                                                 | Data Type     |
|----------------------|:----------------------------------------------------------------------------------------------------------------------------|--------------:|
|MapDate               | Date the measurement was taken                                                                                              | YYYMMDD Format|
|FIPS                  | County Code                                                                                                                 | Integer Format|
|County                | County Name--should all be Bexar                                                                                            |Standard Text  |
|State                 | State Mailing Code                                                                                                          |Standard Text  |
|None                  | Drought level corresponds to "No Drought" describes percent of the county experience this level                             |Standard Number|
|D0                    | Drought level corresponds to "Abnormally Dry" describes percent of the county experience this level                         |Standard Number|
|D1                    | Drought level corresponds to "Moderate Drought" describes percent of the county experience this level                       |Standard Number|
|D2                    | Drought level corresponds to "Severe Drought" describes percent of the county experience this level                         |Standard Number|
|D3                    | Drought level corresponds to "Extreme Drought" describes percent of the county experience this level                        |Standard Number|
|D4                    | Drought level corresponds to "Exceptional Drought" describes percent of the county experience this level                    |Standard Number|
|ValidStart            | Describes the date the drought level began                                                                                  |Standard Number|
|ValidEnd              | Describes the date the drought level ended                                                                                  |Standard Number|

## Of Note
Limitations of a 14 day time constraint to produce a project are as follows:
* Missing Population data- 10 business days to request population data under freedom of information act
* Missing Water consumption data for the J17 well consumers-10 business days to request population data under freedom of information act
* Data cleaning was more extensive than anticipated- each time we would begin to do research, we would find a mismatch in row counts due to previously unforseen issues (missing data, leap year, etc)
* Of course, the 14 day time limit to produce and report on the project
* The newness of the group to data in general
