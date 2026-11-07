# Determining EEZ Priority Zones for Aquaculture

This repository contains materials for the third assignment for [EDS 223 - Geospatial Analysis & Remote Sensing](https://eds-223-geospatial.github.io/). Full instructions for this assignment can be found on [the course website](https://eds-223-geospatial.github.io/assignments/HW3.html). Per instructions, this repo explores suitable areas for potential marine aquaculture species along the West Coast of the US and determines priority Exclusive Economic Zones (EEZ) for these species based on the amount of suitbale area. The suitable area is determined based on range of suitable sea surface temperature (SST) and depth values for the species. The two species explored in this repo are oysters and red abalone. 

## Repository Structure
```
eez-aquaculture
│   README.md
│   eez_analysis.qmd
│   eez_analysis.pdf
│
└───.gitignore
     └───data
         └───average_annual_sst_2008.tif
         └───average_annual_sst_2009.tif
         └───average_annual_sst_2010.tif
         └───average_annual_sst_2011.tif
         └───average_annual_sst_2012.tif
         └───depth.tif
         └───wc_regions_clean.dbf
         └───wc_regions_clean.prj
         └───wc_regions_clean.shp
         └───wc_regions_clean.shx
```

## Data access
The data used can be accessed from Google Drive as a zip file [here](https://drive.google.com/file/d/1u-iwnPDbe6ZK7wSFVMI-PpCKaRQ3RVmg/view?usp=sharing). Suitable SST and depth were obtained from [Sea Life Base](https://www.sealifebase.ca/search.php). SST data was generated from [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php). Bathymetry data characterizing the ocean's depth is collected from [General Bathymetric Chart of the Oceans (GEBCO)](https://www.gebco.net/data-products/gridded-bathymetry-data#area). Finally, EEZ shapefiles were taken from [Marineregions.org](https://www.marineregions.org/eez.php).

## Analysis and Visualization
Script for analysis and visualization for the project can be found in `eez-analysis.qmd` and rendered as `eez-analysis.pdf`. The final code results in a function where an EEZ priority map can be created for any species by inputing the minimum and maximum SST and depth for a given species.

## References
