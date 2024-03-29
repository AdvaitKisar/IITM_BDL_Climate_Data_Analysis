# IITM_BDL_Climate_Data_Analysis
This is a course project from the course CS5830: Big Data Laboratory offered at IIT Madras.

## Aim
This aim of this project is to create a pipeline to extract the Climate Data from [NCEI](https://www.ncei.noaa.gov/) website and find the monthly averages of different parameters across the globe and create plots to visualize this data.

## Procedure
The steps while executing this assignment are as follows:-
1. The first step is a pipeline to fetch the data from the website using Airflow and store it in the archive. It is important to note that the data available is from 1901 to 2024 with more than 80 parameters and hourly readings with each year having details from anywhere between 5-6 stations to 10000+ stations. Hence, only the years 1901, 1911, ..., till 2001, and 2002 to 2024 were considered.
2. The next two steps have to be executed using Airflow and Apache Beam for performing parallel operations and computations.
3. The next step is to arrange the data location-wise with the parameters in an array. This data was again stored in CSV files.
4. The third step is to compute the monthly averages for each month and parameters for each location. This data was also stored in CSV files.
5. The next step is to plot the data in the form of heatmaps. This is to be executed using geopandas and geodatasets.
6. Finally, an animated video is to be made which is optional. This can be either done programmatically or using a software.

## Parameters
The parameters plotted using the available data are as follows:-
1. Hourly Altimeter Setting
2. Hourly Dew Point Temperature
3. Hourly Dry Bulb Temperature
4. Hourly Relative Humidity
5. Hourly Sea Level Pressure
6. Hourly Station Pressure
7. Hourly Visibility
8. Hourly Wet Bulb Temperature
9. Hourly Wind Direction
10. Hourly Wind Speed

## Plots
The plots or heatmaps for the ten parameters are included in the 'Plots' directory. For example, the heatmap of Hourly Sea Level Pressure is shown below:-
![Hourly Sea Level Pressure Heatmap for Jan](https://github.com/AdvaitKisar/IITM_BDL_Climate_Data_Analysis/assets/85425955/1a924297-abf7-445f-bb4c-dcce1fa75fd6)
It can be observed that the sea level pressure in the coastal regions is lower as compared to the interiors of continents. Such observations can be studied using all plots.

## Animations
The animation for the Sea Level Pressure is plotted as shown below:-

https://github.com/AdvaitKisar/IITM_BDL_Climate_Data_Analysis/assets/85425955/065361ef-3853-4420-9e34-37ee400bd423

The animations help us to identify the global patterns which can help in understanding the global climate in much more detailed manner.

Do check out the plots in the 'Plots' directory and animations in the 'Animations' directory.
