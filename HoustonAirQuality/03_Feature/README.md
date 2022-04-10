[BACK TO HAQ MAIN PAGE SUMMARY](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/tree/main/HoustonAirQuality)
<br>
![cover](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/main/HoustonAirQuality/06_Images/HAQ_FEAT_Title.png)

# CONSIDERATIONS
The outdoor air quality data from EPA/Tamis is composed of 6 dataframes, each containing the information about one pollutant: ozone, CO, NO2, SO2, PM 2.5 and PM 10.
The first step of the feature engineering is to clean up the dataframes. The second step addresses potential alternate ways to model the data.
Cleaning up the dataframes involve:
- create month and day columns.
- remove unneeded columns and simplify temperature data by keeping only the maximum temperature
- get dummies on categorical data.
- check columns and drop date index.
- create train/test sets and export files for modeling.

With XGBoost the plan is to model each pollutant individually. I am also interested to see if ozone could be predicted from other pollutants in the following cases:
- one air station records multiple pollutants.
- by date, regardless of station location.

Another interesting test is to try to model using two different y:
- the actual concentration of ozone (i.e. the number ug/m3).
- the AQI category (i.e. safe, moderate, unhealthy...).


picture in the title banner from https://www.smithers.com/resources/2019/feb/future-packaging-trends-2018-to-2028

<br>
[BACK TO HAQ MAIN PAGE SUMMARY](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/tree/main/HoustonAirQuality)
<br>
