*UCSB MEDS* - *EDS 223 - Geospatial Analysis &amp; Remote Sensing*


# West Coast Aquaculture Habitat Suitability Analysis

![R Programming](https://img.shields.io/badge/R_Programming-cornflowerblue?style=for-the-badge&logo=R) ![Remote Sensing](https://img.shields.io/badge/Remote_Sensing-green?style=for-the-badge) ![GIS](https://img.shields.io/badge/GIS-purple?style=for-the-badge)  ![UCSB MEDS](https://img.shields.io/badge/UCSB%20MEDS-blue?style=for-the-badge) 

**Author:** Nicole Pepper

<div style="text-align: left;">
  <img src="https://eds-223-geospatial.github.io/assignments/images/aquaculture.jpg" alt="Image" width="800">

*Image by [Hanson Lu](https://unsplash.com/photos/aerial-photography-of-white-frames-on-top-of-water-eUfnha6ev9g)*

### About the Repo:

[This repository](https://github.com/nicolelpepper/EDS223-aquaculture-habitat-suitability) contains a R-Studio Quarto Markdown document of my analysis identifying the suitability of Exclusive Economic Zones (EEZs) along the U.S. West Coast for developing marine aquaculture using sea surface temperature (SST) and depth below sea level. For this analysis, I create a generalizable function that outputs a map showing EEZ regions colored by the amount of suitable area for aquaculture.

### Technical Highlights:
- Combining vector/raster data
- Resampling & masking raster data
- Raster calculations for determining suitability
- Creating a function for streamlined workflow

### Data Descriptions:

- The `Average Annual Sea Surface Temperature` (SST) data is a collection of raster files containing the Average Annual SST for 2008 - 2012 along the U.S. West Coast. It is from NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly. The SST data is stored in `/data/` folder in the repo as `average_annual_sst_YEAR`, I did not push the original full dataset to GitHub, it was accessed locally.
  
- The `depth` dataset is from General Bathymetric Chart of the Oceans (GEBCO). image from Landsat Collection 2 Level-2, from the Microsof Planetary Computer data catalogue. Landsat Collection 2 Level-2 Science Products consist of atmospherically corrected surface reflectance and surface temperature image data. Collection 2 Level-2 Science Products are available from August 22, 1982 to present. It is accessed through UCSB Workbench 1 `/courses/EDS220/data/hwk4_landsat_data landsat8-2018-01-26-sb-simplified.nc`. 

Habitat Suitability Ranges: sealifebase.ca Access date: 11/20/24

Exclusive Economic Zones (EEZ) Boundaries: Marine Regions Access date: 11/20/24

Sea Surface Temperature NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1 Access date: 11/20/24

Bathymetry: General Bathymetric Chart of the Oceans (GEBCO) Access date: 11/20/24
### Repo structure:

```
EDS223-HW3
│   README.md
│   qmd/Rmd/Proj files
|   .gitignore
│
└───data
    │   wc_regions_clean.shp
    │   depth.tif
    │   average_annual_sst_2008.tif
    │   average_annual_sst_2009.tif
    │   average_annual_sst_2010.tif
    │   average_annual_sst_2011.tif
    │   average_annual_sst_2012.tif
```

### References:

- Habitat Suitability Ranges: [sealifebase.ca](https://www.sealifebase.ca/search.php) *Access date: 11/20/24*

- Exclusive Economic Zones (EEZ) Boundaries: [Marine Regions](https://www.marineregions.org/eez.php) *Access date: 11/20/24*

- Sea Surface Temperature [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php) *Access date: 11/20/24*

- Bathymetry: [General Bathymetric Chart of the Oceans (GEBCO)](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area) *Access date: 11/20/24*

### Acknowledgments:

This assignment was created by Ruth Oliver, EDS 223 - Fall 2024 Instructor.
