# sea-level-sensors-frontiers
Smart Sea Level Sensors - additional project info:
https://www.sealevelsensors.org/

This repository provides the code used to conduct the data analysis and create the figures in the SSLS proposal to Frontiers in Marine Science. 

api_scraper.py is used to make calls to the Sea Level Sensors API and the Tides and Currents NOAA API. 

SSLS-Frontiers_Analysis.ipynb 

1) DATA ACQUISITION: The program first utilizes api_scraper.py to acquire Sea Level Sensor data and NOAA Tide Gauge data. The NOAA Tide Gauge at Fort Pulaski is utilized as a benchmark for water levels in that region as the only long-standing tide gauge, so the Smart Sea Level Sensor team co-located two sensors on the Fort Pulaski dock by the Tide Gauge. These three timeseries are seen plotted together.

2) ERROR ANALYSIS USING RESIDUALS: The two co-located sensors at Fort Pulaski are compared to the NOAA Tide Gauge by calculating the residual between each sensor and the Tide Gauge. Reproducability of the two co-located sensors is also calculated. Time series are plotted with residuals.

3) SPATIAL ANALYSIS: The Smart Sea Level Sensor network seeks to help in understanding the spatial variance of tide cycles and water levels throughout the region. Tide cycles seen at each sensor location are studied and compared to the NOAA Tide Gauge benchmark to understand the water level offsets and time delays associated to the region.

4) HURRICANE DORIAN CASE STUDY: Understanding how the sensor network and tidal cycles respond to extreme events is vital to the purpose of this project. Hurrican Dorian is studied by conducting spatial analysis during the two weeks surrounding the hurricane. Effects of rain and wind are also considered in this analysis. 

Reference APIs:

https://dev.sealevelsensors.org/

https://tidesandcurrents.noaa.gov/waterlevels.html?id=8670870
