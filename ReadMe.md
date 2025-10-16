# HPAI in Canada: Discovering Hot and Cold Spots and Environmental Drivers

This repository provides dataset for spatial analysis of Highly Pathogenic Avian Influenza (HPAI) in Canada. 
HPAI outbreaks have increased worldwide in recent years, creating significant challenges for animal health, food security, and the poultry sector. Understanding the spatial distribution of outbreaks and the environmental factors that influence them is essential for effective monitoring and control. This study contributes to that objective by conducting a detailed spatial assessment of HPAI occurrences across Canada, pinpointing regions at elevated risk and identifying the primary environmental and agricultural determinants linked to disease emergence. The results provide actionable knowledge to strengthen targeted surveillance, improve biosecurity measures, and inform science-based policy and management decisions within a One Health context.

This repository includes date form x varous sources that are explained below:
- **Air Qulity:** In the Air Qulity folder, the minimum, maximum, and mean concentration of 9 different parameters, namely, CH4, CO, NO2, SO2, O3, HCHO, H2O, UV-index, and cloud density, are available for Canada on subdivision level. The data which is collected form [Sentinel-5P of Google Earth Engine (GEE)](https://developers.google.com/earth-engine/datasets/catalog/sentinel-5p), is presented from Jan 1, 2021 to Jan 1, 2025, on 4 months basis. The columns of each file in this folder include:
    * CCSNAME: Stands for Census Consolidation Subdivision Name
    * CSDNAME: Stands for Census SubDivision Name
    * CSDTYPE: A code that indicates the type of the Subdivision.
    * CSDUID: Census Subdivision Unique Identifier
    * DGUID: Dessimination Geography Unique Identifier
    * LANDAREA: The site area of the subdivision
    * PRUID: The province Identifier
    * max: Maximum concentration of the air quality parameter
    * mean: Mean concentration of the air quality parameter
    * min: Minimum concentration of the air quality parameter
    * start_date: The date marking the beginning of data collection
    * end_date: The date marking the end of data collection
    * Parameter: The air quality parameter
- **Weather:** 

