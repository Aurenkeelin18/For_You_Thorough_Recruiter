![cover](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/f9c581996bba87893810a54c314a6c1c8a62f395/HoustonAirQuality/06_Images/HAQ_EDA_Title.png)

## AIR QUALITY INDEX (AQI)
The AQI, which is calculated using measured pollutant concentrations, describes the impact of pollution on the quality of life and daily activities. When applied to ozone concentrations the effects are as described in the picture below. 
<br>

![tv](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/95b676f5c45e343360020798a018b9f1604f10d4/HoustonAirQuality/06_Images/HAQ_AQI.png)

![AQI](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/b29e1f1aac22f66c4c378478dc4c9de0d741509a/HoustonAirQuality/06_Images/HAQ_AQICalculation.png)

## INDOOR DATA 1999-2001 (RIOPA)
Although it was quite exciting to attemp modeling indoor data from outdoor data, the RIOPA dataset did not provide enough information, consequently the idea was dropped.

<br>

![riopa](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/5d4af71ab19981782fb6df27cdeef3fbfce7b0a8/HoustonAirQuality/06_Images/HAQ_EDA_slide1.png)
<br>
## THE MOST CONCERNING POLLUTANTS IN OUTDOOR DATA
The Exploratory Data Analysis shows that between 2008 and 2020 Ozone is the  problematic pollutant in Houston. The other pollutants remain in the “safe” zone and rarely go up to moderate if ever. Despite BADs, the weekly and monthly average ozone concentrations remain mostly in the “safe” zone.

![slide2](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/5d4af71ab19981782fb6df27cdeef3fbfce7b0a8/HoustonAirQuality/06_Images/HAQ_EDA_slide2.png)


## BADs AT A GLANCE (2008-2020)
There is an average of 129 BADs per year which may be as low as “Moderate” (80-110 days per year) up to “Very Unhealthy” (1 to 2 days per year). Ozone levels are lower in Winter and Spring.

![slide3](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/5d4af71ab19981782fb6df27cdeef3fbfce7b0a8/HoustonAirQuality/06_Images/HAQ_EDA_slide3.png)


## IT LOOKS BAD BUT IT IS NOT BADs

Interestingly the EDA showed that severe weather or special events as bad as they look did not lead to a BAD.
* **Hurricanes:** Harvey (August 25-29th, 2017 - cat 4) and Ike (September 13th, 2008 - cat 2) lead to very little records during the event because the air quality stations are turned off and sheltered. There was no rebound of or decrease in  pollution after the event.

![harvey](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/5d4af71ab19981782fb6df27cdeef3fbfce7b0a8/HoustonAirQuality/06_Images/HAQ_EDA_slide4.png)
<br>

* **Flooding:** Tropical Storm Imelda (September 19th, 2019) and Memorial Day Flood (May 25-26th, 2015 - 11 inches of rain in 9 hours) do not disturb the records.

* **Chemical Plant Fire:** Deerpark ITC fire (March 17-20th 2019) lasted several days and released a large plume of smoke that covered Houston but the PM pollutant records (VOCs might have spiked).

* **Pandemic:**  'Stay Home' order (start sign) during the Covid-19 outbreak (March 16th - April 30th 2020) helped ozone to reach very low levels in March until March 24th which was the day after the media announced that Judge Hidalgo would declare a “Stay at Home” order (plus sign) to replace the “Shelter in Place” order.

![pandemic](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/5d4af71ab19981782fb6df27cdeef3fbfce7b0a8/HoustonAirQuality/06_Images/HAQ_EDA_slide6.png)

* **Saharan Dust Storm:**  The Dust Storms always make the news especially in August 6th-8th 2013 and in June 2020 when the dust haze was highly visible (see picture below). The particulate matter PM 10 barely reached “Moderate” while PM 2.5 remains in the safe zone.

![dust](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/5d4af71ab19981782fb6df27cdeef3fbfce7b0a8/HoustonAirQuality/06_Images/HAQ_EDA_slide5.png)



## EDA CONCLUSIONS
The EDA showed that there are no direct or 'easy' relationships between pollutants and their environmental and human-driven factors. Ozone is the pollutant which is the most obvious to interpret from concentration data. Binned traffic and population growth data may help unravel patterns between ozone and  its precursors (i.e. NO2, CO), and insights about the drivers of pollutants formation and distribution in Houston.
Other considerations that have not been shown here but will be evaluated with the model are:
* most and least polluted day of the week.
* most and least polluted month.
* special events leading to pollution (e.g. Thanksgiving, 4th of July, Labor Day...)
* lag between ozone preucrsor release and ozone formation.



picture in the title banner from https://cdn.images.express.co.uk/img/dynamic/151/590x/sun-magnify-780580.jpg
