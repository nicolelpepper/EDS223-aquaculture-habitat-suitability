*UCSB MEDS* - *EDS 223 - Geospatial Analysis &amp; Remote Sensing*


# Aquaculture Habitat Suitability Analysis

**Author:** Nicole Pepper

**Link to github repo:** https://github.com/nicolelpepper/EDS223-aquaculture-habitat-suitability

![R Programming](https://img.shields.io/badge/R_Programming-cornflowerblue?style=for-the-badge&logo=R)  ![Remote Sensing](https://img.shields.io/badge/Remote_Sensing-green?style=for-the-badge)  ![GIS](https://img.shields.io/badge/GIS-purple?style=for-the-badge)  

 ![ Image](https://eds-223-geospatial.github.io/assignments/images/aquaculture.jpg)

Image by [Hanson Lu](https://unsplash.com/photos/aerial-photography-of-white-frames-on-top-of-water-eUfnha6ev9g)

### About the assignment:

For this project, I identify the best Exclusive Economic Zones (EEZs) along the U.S. West Coast for developing marine aquaculture using sea surface temperature (SST) and depth requirements to determine suitability. I create a generalizable function that outputs a map showing EEZ regions colored by the amount of suitable area for aquaculture:

**Technical Highlights:**
- combining vector/raster data
- resampling & masking raster data
- raster calculations for determining suitability
- creating a function for streamlined workflow

### About this repo:

This repository contains a notebook `hwk4-task2-fire-perimeter-PEPPER.ipynb` that subsets the historic california fire boundary dataset to the Thomas Fire Boundary and a notebook `hwk4-task2-false-color-PEPPER.ipynb` exploring the burn scar for the 2017 Thomas Fire in Santa Barbara and Ventura Counties in California. For the assignment, I visualize a satellite image over the burn area in false color to highlight the burn scar and overlay it with the outline of the Thomas Fire burn perimeter.

### Datasets descriptions:

- The `thomas_fire.shp` is a shapefile containing the fire perimeter for the Thomas Fire in 2017. It is subset of a CAL FIRE dataset with historical boundaries for fires (including both natural and prescribed fires) in the state of California. The dataset has a good record of past large fires but is not complete and may be missing some fires. The thomas_fire.shp data is stored in `/data/thomas_fire` folder in the repo, I did not push the original full Cal Fire dataset to GitHub, it was accessed locally.
  
- The `landsat.nc` dataset is an image from Landsat Collection 2 Level-2, from the Microsof Planetary Computer data catalogue. Landsat Collection 2 Level-2 Science Products consist of atmospherically corrected surface reflectance and surface temperature image data. Collection 2 Level-2 Science Products are available from August 22, 1982 to present. It is accessed through UCSB Workbench 1 `/courses/EDS220/data/hwk4_landsat_data landsat8-2018-01-26-sb-simplified.nc`. 

### References:

CAL FIRE (2024) *California Fire Perimeters (all)* [Data file] Available from: https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436 Access date: 11/20/24

USGS (2024) *Landsat Collection 2 Level-2 Surface Reflectance and Surface Temperature Products* [Data file]. Available from: https://www.usgs.gov/landsat-missions/landsat-collection-2 Access date: 11/20/24

Carmen Galaz García (2024) *UCSB MEDS - 220 - Working With Environmental Datasets * [Source of Homework Assignment]. Course Website: https://meds-eds-220.github.io/MEDS-eds-220-course/ Access date: 11/20/24

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

### Acknowledgments:

This assignment was created by Ruth Oliver, EDS 223 - Fall 2024 Instructor.
