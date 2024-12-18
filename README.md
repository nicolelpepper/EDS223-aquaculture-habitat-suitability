*UCSB MEDS* - *EDS 223 - Geospatial Analysis &amp; Remote Sensing*


# West Coast Aquaculture Habitat Suitability Analysis

![R Programming](https://img.shields.io/badge/R_Programming-cornflowerblue?style=for-the-badge&logo=R) ![Remote Sensing](https://img.shields.io/badge/Remote_Sensing-green?style=for-the-badge) ![GIS](https://img.shields.io/badge/GIS-purple?style=for-the-badge)  ![UCSB MEDS](https://img.shields.io/badge/UCSB%20MEDS-blue?style=for-the-badge) 

**Author:** Nicole Pepper

<div style="text-align: left;">
  <img src="https://eds-223-geospatial.github.io/assignments/images/aquaculture.jpg" alt="Image" width="700">

*Image by [Hanson Lu](https://unsplash.com/photos/aerial-photography-of-white-frames-on-top-of-water-eUfnha6ev9g)*

### About the Repo:

[This repository](https://github.com/nicolelpepper/EDS223-aquaculture-habitat-suitability) contains a R-Studio Quarto Markdown document of my analysis identifying the suitability of Exclusive Economic Zones (EEZs) along the U.S. West Coast for developing marine aquaculture using sea surface temperature (SST) and depth below sea level. For this analysis, I create a generalizable function that outputs a map showing EEZ regions colored by the amount of suitable area for aquaculture.

### Technical Highlights:
- Programming in R
- Vector data wrangling with `sf`
- Raster data wrangling with `terra` and `stars`
- Data visualization with `tmap` and `ggplot`
- Creating a function for streamlined workflow

### Data Descriptions:

- The `Average Annual Sea Surface Temperature` (SST) data is a collection of raster files containing the average annual SST for 2008 - 2012 along the U.S. West Coast. It is from NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly. The SST data is stored in `/data/` folder in the repo as `average_annual_sst_YEAR.tif`, I did not push the original full dataset to GitHub, it was accessed locally.
  
- The `Depth` dataset is from General Bathymetric Chart of the Oceans (GEBCO). The SST data is stored in `/data/` folder in the repo as `depth.tif`, I did not push the original full dataset to GitHub, it was accessed locally.

- The `Exclusive Economic Zone (EEZ) Boundary` data is from Marine Regions.  The EEZ data is stored in `/data/` folder in the repo as `wc_regions_clean.shp`, I did not push the original full dataset to GitHub, it was accessed locally.

- The `State Boundary` dataset is from TIGER/Line Shapefiles. R package `TIGRIS` version 1.5.0. https://CRAN.R-project.org/package=tigris.
  
### Repo structure:

```
aquaculture-habitat-suitability
│   README.md
│   qmd/Rmd/Proj files
|   .gitignore
│
└───data
│      │   wc_regions_clean.shp
│      │   depth.tif
│      │   average_annual_sst_2008.tif
│      │   average_annual_sst_2009.tif
│      │   average_annual_sst_2010.tif
│      │   average_annual_sst_2011.tif
│      │   average_annual_sst_2012.tif
│
└───images
       aquaculture-cover-photo.jpg
```

### References:

- [sealifebase.ca](https://www.sealifebase.ca/search.php) [Data] *Access date: 11/20/24*

- [Marine Regions](https://www.marineregions.org/eez.php) [Data] *Access date: 11/20/24*

- [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php) [Data] *Access date: 11/20/24*

- [General Bathymetric Chart of the Oceans (GEBCO)](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area) [Data] *Access date: 11/20/24*

- [TIGER/Line Shapefiles version 1.5.0](https://CRAN.R-project.org/package=tigris) [Data] *Access date: 11/20/24*


### Acknowledgments:

This assignment was created by Ruth Oliver, EDS 223 - Fall 2024 Instructor.
