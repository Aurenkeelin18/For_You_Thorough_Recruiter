![cover](HoustonAirQuality/06_Images/HAQ_DW_Title.png)


picture from https://fr.wikipedia.org/wiki/Jeu_de_billes#/media/Fichier:WestAfricanMarbles.jpg

## Bad Air Days (BADs) In The Daily Life Of Houstonians

![first](./06_Images/HAQ_DW_slide1.png)


## Pollutants and Air Quality Index

![second](./06_Images/HAQ_DW_slide2.png)


## The Hypothesis, The Data, The Plan

![third](./06_Images/HAQ_DW_slide3.png)


## Thinking the Dataset And Data Wrangling
The idea is to merge the data into a coherent data set by taking into account geographical locations, and by covering as much territory possible from The Woodlands to the North all the way down to Galveston to the Southeast on the coastline, including Baytown and Angleton (plants). <br>
![fourth](./06_Images/HAQ_DW_slide4.png)
<br>
The main issues encountered during the wrangling of the data were:
..* Matching sampling rates: the sampling rate (i.e. how many times a day or how long the sampling is) differs between pollutants. Only full daily records were kept following the way TCEQ reports to EPA (i.e. maximum values),<br>
..* Connect local weather to each air quality station:  the weather data comes from three weather stations with N, SE and central locations,<br>
..* Deal with missing data: using appropriate imputation (time series driven) or by discarding the “day”.  Another problem was that the RIOPA data did not contain the location of the homes where indoor air sampling occurred. Consequently, the RIOPA model could not be connected to the outdoor air quality model,<br>
..* Traffic: Yearly traffic count was linked to the air quality stations within Manhattan distance of the traffic data point, subsequently summed and binned,<br>
..* Population: the data was integrated to the data set in term of “% growth” per year per neighborhood. The data was binned linked to the air quality stations within Manhattan distance,<br>
 ..* Land use: Houston is a mozaique of land use (i.e. no zonation) and therefore the notion of land use “near” another land use was added to the land use at the location (e.g. residential near land use).  For instance, a given air quality station can be  “Residential” and “Residential near Industrial”.<br>







