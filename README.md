# A Review of the Effectiveness of the San Antonio Water System (SAWS) Water Restrictions Policies
## Overview
The topic was chosen as a starter project for the contributors to apply the skills they have attained in their Data Analytics Bootcamp. This is the first group project of the bootcamp, and as such- the scope will be very limited. Many contributors are new to either data analytics or math, or both. The limitation of the scope enables the contributors to apply the knowledge learned without the additional anxiety of needing to apply things they have not yet learned. 
The group of contributors are located within the San Antonio area, and-like many in the area-find the city seems to be under water restrictions daily. With this in mind, they decided to investigate the determining factors driving these restrictions. Were the water restrictions helping to replenish the well, keep it at a steady level, or was the water level decreasing regardless of these restrictions.
## Variable Determination
Drought information- when in D1 or higher, does the J17WL well water level increase, decrease or remain constant -to determine if water restrictions are effective
Quantitative effect of temperature on the water levels--> this is to say perhaps SAWS could implement something more strict to prevent water level dropping during high temps?
Quantitative effect of humidity on the water levels and drought levels-->this is for fun to see if there are +/- correlations between drought or water levels and humidity -->maybe extrapolate a finding that when humidity is high and we are in drought- that water restrictions are not as necessary as when humidity is low?
## Findings
Insert findings here
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

## Other forgotten things
