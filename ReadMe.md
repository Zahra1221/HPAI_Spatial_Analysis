# HPAI in Canada: Discovering Hot and Cold Spots and Environmental Drivers

This repository provides dataset for spatial analysis of Highly Pathogenic Avian Influenza (HPAI) in Canada. 
HPAI outbreaks have increased worldwide in recent years, creating significant challenges for animal health, food security, and the poultry sector. Understanding the spatial distribution of outbreaks and the environmental factors that influence them is essential for effective monitoring and control. This study contributes to that objective by conducting a detailed spatial assessment of HPAI occurrences across Canada, pinpointing regions at elevated risk and identifying the primary environmental and agricultural determinants linked to disease emergence. The results provide actionable knowledge to strengthen targeted surveillance, improve biosecurity measures, and inform science-based policy and management decisions within a One Health context.

This repository includes date form x varous sources that are explained below:
- **Air Qulity:** In the Air Qulity folder, the maximum concentration of 9 different parameters, namely, CH4, CO, NO2, SO2, O3, HCHO, H2O, UV-index, and cloud fraction, are available for Canada on subdivision level. The data which is collected form [Sentinel-5P of Google Earth Engine (GEE)](https://developers.google.com/earth-engine/datasets/catalog/sentinel-5p), is presented from Jan 1, 2021 to Jan 1, 2025, on 4 months basis. The columns of each file in this folder include:
    * CCSNAME: Stands for Census Consolidation Subdivision Name
    * CSDNAME: Stands for Census SubDivision Name
    * CSDTYPE: A code that indicates the type of the Subdivision.
    * CSDUID: Census Subdivision Unique Identifier
    * DGUID: Dessimination Geography Unique Identifier
    * LANDAREA: The site area of the subdivision
    * PRUID: The province Identifier
    * max: Maximum concentration of the air quality parameter over the subdivision
    * mean: Mean concentration of the air quality parameter over the subdivision
    * min: Minimum concentration of the air quality parameter over the subdivision
    * start_date: The date marking the beginning of data collection
    * end_date: The date marking the end of data collection
    * Parameter: The air quality parameter
- **Weather:** From [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api) two daily weather parameters, namely Minimum Temperature (2 m) and Rain Sum were collected on approxcimately 333 Km resolution for Canada. Minimum temperature was averaged over a 4 year period (2021-01-01 to 2025-01-01), and Rain was summed over each year (i.e. 2021, 2022, 2023, 2024), and then averaged over all the years. Next, these data were spatially interpolated in ArcGIS pro using the ordinary kriging method to transform it into a 232 m resolution. This resolution is enough to have at least 1 value in each subdivision. The columns of this dataset include:
    * CSDUID: Census Subdivision Unique Identifier
    * DGUID: Dessimination Geography Unique Identifier
    * CSDNAME: Stands for Census SubDivision Name
    * CSDTYPE: A code that indicates the type of the Subdivision.
    * LANDAREA: The site area of the subdivision
    * PRUID: The province Identifier
    * CCSNAME: Stands for Census Consolidation Subdivision Name
    * temperature_min: Temperature, minimized over each subdivision
    * temperature_max: Temperature, maximized over each subdivision
    * temperature_mean: Temperature, averaged over each subdivision
    * rain_min: Rain, minimized over each subdivision
    * rain_max: Rain, maximized over each subdivision
    * rain_mean: Rain, averaged over each subdivision
- **Wildfire:** It was collected from [Google Earth Engine Firms](https://developers.google.com/earth-engine/datasets/catalog/FIRMS) from 2021-01-01 to 2025-01-01 on 4 months bases. Each entry of the dataset includes the maximum of the fire value over the 4 months period. The columns include:
    * CCSNAME: Stands for Census Consolidation Subdivision Name
    * CSDNAME: Stands for Census SubDivision Name
    * CSDTYPE: A code that indicates the type of the Subdivision.
    * CSDUID: Census Subdivision Unique Identifier
    * DGUID: Dessimination Geography Unique Identifier
    * LANDAREA: The site area of the subdivision
    * PRUID: The province Identifier
    * max: Maximum fire value over the subdivision
    * mean: Mean fire value over the subdivision
    * min: Minimum fire value over the subdivision
    * start_date: The date marking the beginning of data collection
    * end_date: The date marking the end of data collection
- **Elevation:** 

