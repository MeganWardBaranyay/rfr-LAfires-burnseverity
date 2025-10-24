# rfr-lafires-emit-ecostress_burnseverity
Random Forest regression model for predicting burn severity (dNBR) from multi-sensor remote sensing data, integrating EMIT and ECOSTRESS fuels conditions, fire weather, and topography across three of the January 2025 Los Angeles County wildfires.

**Data Availability**

- ECOSTRESS Collection 2 Level 3 and 4 products and orthorectified EMIT Level 2A Surface Reflectance were retrieved from the Application for Extracting and Exploring Analysis Ready Samples (AppEEARS) (https://appeears.earthdatacloud.nasa.gov/). 

  - ECOSTRESS resampling and Canopy Water Content estimation was performed using code available at the NASA VITALS repository ([nasa.github.io/VITALS/](https://nasa.github.io/VITALS/)).

- The Shuttle Radar Topography Mission (SRTM)-derived elevation, aspect, and slope were retrieved from OpenTopography (https://doi.org/10.5069/G9445JDF). 

- The NOAA Real-Time Mesoscale Analysis (RTMA) data products were retrieved using Google Earth Engine (https://developers.google.com/earth-engine/datasets/catalog/NOAA_NWS_RTMA#bands).

- Vapor pressure deficit (VPD) was retrieved from ClimateEngine.org (https://app.climateengine.org/climateEngine).

- The National Land Cover Database (NLCD) product and Landsat 8 imagery for computing dNBR were retrieved from USGS EarthExplorer (https://earthexplorer.usgs.gov/). 

- Random forest regression modelling was performed with the scikit-learn RandomForestRegressor (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html).

*All data and code to run the model and produce figures are available in the "Data" folder.* 


The code is designed to run within the **[NASA VITALS environment](https://github.com/nasa/VITALS)**, which provides the standardized dependencies and environment configuration for the workflow.
