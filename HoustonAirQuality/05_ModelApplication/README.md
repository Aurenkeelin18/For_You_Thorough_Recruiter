[BACK TO HAQ MAIN PAGE SUMMARY](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/tree/main/HoustonAirQuality)
<br>
![cover](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/main/HoustonAirQuality/06_Images/HAQ_MAPP_Title2.png)

## INDIVIDUAL CONTRIBUTIONS OF FACTORS
The model is used to see what would happen to ozone concentrations levels (low, average and BADs) when the major drivers increase or decrease. For this the degrees are added or removed from the maximum temperature while the wind speed and total precipitation are multiplied by a factor. 
* **Temperature** is a catalyzer on all levels of ozone though,
* **High winds** play a dual role of dispersion on high level of ozone but tends to catalyze ozone formation in zones where ozone is low. 
* **Rain seems** to have no influence by itself.


![slide1](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/main/HoustonAirQuality/06_Images/HAQ_MAPP_slide1.png)

## DRIVERS AND BUFFERS
There is a very interesting game of buffer and driver between temperature and wind speed. High wind speeds tend to buffer the action of higher temperature which can be explained by the role of dispersion of the wind (i.e. dispersion of the ozone and also the dispersion of the chemicals involved in its formation). For instance, at the highest temperature (+15F) increasing the wind speed by 50% helps shifting the air quality from “Very Unhealthy” to “Unhealthy”.

![slide2](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/main/HoustonAirQuality/06_Images/HAQ_MAPP_slide2.png)


## CONCLUSIONS

![slide3](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/main/HoustonAirQuality/06_Images/HAQ_MAPP_slide3.png)

It is very difficult for data scientists to avoid being biased by the data and their personal opinion or experience when preparing datasets to build a model. I am sure my bias came from the many hours during which I got stuck in traffic in Houston, the many hours of small talk about traffic, and the numerous and recurring news and headlines about traffic, haze, smog...etc... 
The data said "No".
The model said "Let me show you what it is about".
Using the XGB Regressor, the results could have been better if the data was just focussed on collecting pollutant, including VOCs, and weather data, skipping population and traffic. Even if the metrics of the model are not ideal or optimum, the model reveals interesting and somewhat releaving trends. 

The most concerning pollutant in Houston is ozone. The hypothesis saying that more people in Houston would lead to more traffic and hence more pollution was wrong. The main driver of ozone pollution is the maximum outdoor temperature followed by wind speed.
The model is built to show trends as opposed to predict daily values. The MAE metric works for this purpose.

The model can help explore the influence of the drivers of ozone concentrations and  also how they can catalyze or buffer each other. The model also can be used to predict the number and intensity of BADs due to ozone.

Increasing maximum temperatures tend to increase ozone concentrations while increasing average and fastest wind act as a buffer. The wind seems to disperse the ozone or the chemicals leading to ozone.

There are many ways the model can be improved: 
* Traffic and population could be integrated differently,
* The surface and geographical frequency of land use could be added.
* VOCs emission could be added, which is part of the ozone formation equation.
* Industrial emission could be added, if available with geographical details.
* The imbalance of the AQI labels could be overcome using a Deep Learning model.

You may find the PowerPoint and pdf reoprts [here](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/main/HoustonAirQuality/07_Reports/)




picture in the titla banner from Salvado Dali https://www.phillips.com/detail/salvador-dali/NY030012/64

<br>
[BACK TO HAQ MAIN PAGE SUMMARY](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/tree/main/HoustonAirQuality)
<br>
