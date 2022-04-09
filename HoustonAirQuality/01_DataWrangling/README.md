![cover](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/311f14d30588400fa591b2cc3dc0ca7733a2ccb5/HoustonAirQuality/06_Images/HAQ_DW_Title.png)

<br>
## Bad Air Days (BADs) In The Daily Life Of Houstonians

![first](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/9b870975c5c4eb6dfb8c23cc9e8140d63a72402b/HoustonAirQuality/06_Images/HAQ_DW_slide1.png)


<br>
## Pollutants and Air Quality Index

![second](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/9b870975c5c4eb6dfb8c23cc9e8140d63a72402b/HoustonAirQuality/06_Images/HAQ_DW_slide2.png)


<br>
## The Hypothesis, The Data, The Plan

![third](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/9b870975c5c4eb6dfb8c23cc9e8140d63a72402b/HoustonAirQuality/06_Images/HAQ_DW_slide3.png)


<br>
## Thinking the Dataset And Data Wrangling
The idea is to merge the data into a coherent data set by taking into account geographical locations, and by covering as much territory possible from The Woodlands to the North all the way down to Galveston to the Southeast on the coastline, including Baytown and Angleton (plants). <br>
![fourth](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/9b870975c5c4eb6dfb8c23cc9e8140d63a72402b/HoustonAirQuality/06_Images/HAQ_DW_slide4.png)
<br>
The main issues encountered during the wrangling of the data were:
* Matching sampling rates: the sampling rate (i.e. how many times a day or how long the sampling is) differs between pollutants. Only full daily records were kept following the way TCEQ reports to EPA (i.e. maximum values).<br>
..* **Connect local weather to each air quality station:**  the weather data comes from three weather stations with N, SE and central locations,<br>
..* **Deal with missing data:** using appropriate imputation (time series driven) or by discarding the “day”.  Another problem was that the RIOPA data did not contain the location of the homes where indoor air sampling occurred. Consequently, the RIOPA model could not be connected to the outdoor air quality model,<br>
..* **Traffic:** Yearly traffic count was linked to the air quality stations within Manhattan distance of the traffic data point, subsequently summed and binned,<br>
..* **Population:** the data was integrated to the data set in term of “% growth” per year per neighborhood. The data was binned linked to the air quality stations within Manhattan distance,<br>
 ..* **Land use:** Houston is a mozaique of land use (i.e. no zonation) and therefore the notion of land use “near” another land use was added to the land use at the location (e.g. residential near land use).  For instance, a given air quality station can be  “Residential” and “Residential near Industrial”.<br>


picture in the title banner from https://fr.wikipedia.org/wiki/Jeu_de_billes#/media/Fichier:WestAfricanMarbles.jpg
