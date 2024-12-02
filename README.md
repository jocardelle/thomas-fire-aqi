# Visualizing the effects of the 2017 Thomas Fire in Santa Barbara County

[Github Repository](https://github.com/jocardelle/thomas-fire-aqi)

## About

The Thomas Fire, which burned across Santa Barbara and Ventura counties in December 2017, has been one of California’s largest wildfires, devastating over 280,000 acres of land. The fire started on December 4, 2017 and was considered contained on January 2, 2018. In this task, I first used [Air Quality Index (AQI)](https://www.airnow.gov/aqi/aqi-basics/) data from the [US Environmental Protection Agency](https://www.epa.gov) to visualize the impact on the AQI of the 2017 [Thomas Fire](https://en.wikipedia.org/wiki/Thomas_Fire) in Santa Barbara County. I then visualized the effects of the fire on the land through using true and false color imagery.

![](images/thomas_fire_palms.jpeg)

<p style="text-align:center; font-style:italic; color:gray;">Palm trees are consumed by the Thomas Fire. Photo credit: <a href="https://www.latimes.com/local/lanow/la-me-thomas-fire-santa-barbara-fire-20171210-story.html" target="_blank">Marcus Yam / Los Angeles Times</a></p>


## Repository Structure
```
|── thomas-fire-sb  
|└── README.md
|└── thomas_fire_aqi.ipynb
|└── thomas_fire_imagery.ipynb
|└── images/  
|  └── thomas_fire_palms.jpeg 
|└── .gitignore  
|  └── data/ 
|    └── California_Fire_Perimeters 
|      └── California_Fire_Perimeters_(all).cpg
|      └── California_Fire_Perimeters_(all).dbf
|      └── California_Fire_Perimeters_(all).prj
|      └── California_Fire_Perimeters_(all).shp
|      └── California_Fire_Perimeters_(all).shp.xml
|      └── California_Fire_Perimeters_(all).shx
|    └── landsat8-2018-01-26-sb-simplified.nc 
```


## Data
The first two data sets used were [Air Quality Index (AQI)](https://www.airnow.gov/aqi/aqi-basics/) data from the [US Environmental Protection Agency](https://www.epa.gov). They contain information regarding daily AQI by county in 2017 and 2018.

The landsat data was obtained from https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2 and is from January 26, 2018. The fire perimeter data is from https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436 and was accessed through the server at `/courses/EDS220/data/hwk4_landsat_data landsat8-2018-01-26-sb-simplified.nc`. It contains the spatial distribution of large fires in California and was pre-processed to remove data outside land and coarsen the spatial resolution.

The AQI datasets are available to download via the url. The fire perimeter data and landsat data were downloaded into the data folder from the websites provided above.

## References

1. Daily AQI by County for 2017
U.S. Environmental Protection Agency. (n.d.). Daily air quality index (AQI) by county: 2017 [Data set]. Air Quality System (AQS) Data Mart. Retrieved December 1, 2024, from https://aqs.epa.gov/aqsweb/airdata/download_files.html#AQI

2. Daily AQI by County for 2018
U.S. Environmental Protection Agency. (n.d.). Daily air quality index (AQI) by county: 2018 [Data set]. Air Quality System (AQS) Data Mart. Retrieved December 1, 2024, from https://aqs.epa.gov/aqsweb/airdata/download_files.html#AQI

3. California Fire Perimeters
U.S. Geological Survey. (n.d.). California Fire Perimeters - All. Data.gov. Retrieved November 17, 2024, from https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436

4. Landsat Collection 2 Level 2 Data
Microsoft Planetary Computer. (n.d.). Landsat Collection 2 Level 2 Dataset. Retrieved December 1, 2024, from https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2
