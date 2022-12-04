---
output:
  pdf_document: default
  html_document: default
---
# Adapting to the recent changes in R spatial packages (sf, terra, PROJ library) (PROJ03)

*December 8-9, 2022 (9:00-17:00 CET - [https://time.is/CET](https://time.is/CET))*

## Instructor 

Jakub Nowosad (https://jakubnowosad.com/) 

## Course Overview

R statistical software is becoming increasingly popular for spatial analysis and mapping. This is partially due to a large number of R packages devoted to applying various spatial methods. These packages, however, are being revised, updated, or even superseded to allow for better performance, simpler user interface, or expanded capabilities. Substantial recent changes in R spatial packages include developing the ‘sf’ package as a successor of ‘sp’, creation of `terra` as a successor of `raster`, and establishing the `stars` package. Additionally, all of these packages were affected by the recent major updates of the PROJ library. In this course, we will learn to use key packages for the analysis of spatial data, both vector (‘sf’) and raster (‘terra’), and see how they differ from their older counterparts, ‘sp’ and ‘raster’. Another important aspect of the course will be to understood spatial projections and coordinate systems, how the recent PROJ changes affect R users, and how to adjust to them.

By the end of the course, participants should:

- Understand the basic concepts behind spatial analysis ecosystem in R
- Know how packages such as sp/rgeos/rgdal/raster differ from their successors sf/terra/star
- Be able to switch from using packages such as sp/rgeos/rgdal/raster to sf/terra/stars
- Understood the basic concepts behind spatial projections, and how PROJ.7 differs from PROJ4
- Know how to deal with coordinate reference systems in R
- Have the confidence to switch from PROJ4 to PROJ7 (i.e., for instance, adjusting old scripts based on PROJ4)?
    
## Course Programme:

Overview of spatial analysis ecosystem in R

- available R packages for spatial analysis in R
- how do R packages represent spatial objects, and how are they connected with each other
- importance of using the more recent R spatial packages, such as ‘sf’ or ‘terra’
- main concepts behind map projections (geoids, datums, geographic/projected coordinates, types of projections, etc.)
- implementation of these concepts in the PROJ library (used by most R spatial packages)
- differences between PROJ.4 and its newer versions (e.g. PROJ.7)

Spatial vector data analysis in R

- spatial vector data processing & analysis in R
- read/write/and visualize spatial vector data
- differences between ‘sp’/’rgdal’/’rgeos’ and ‘sf’
- moving from ‘sp’ to ‘sf’ for spatial vector data processing & analysis
- spherical geometry: how this concept was recently implemented in sf, and what is an impact of this implementation

Spatial raster data analysis in R

- spatial raster data processing & analysis in R
- read/write/and visualize spatial raster data
- differences between ‘raster’ and ‘stars’/’terra’
- moving from ‘raster’ to ‘terra’ for spatial raster data processing & analysis
- short overview of package ‘stars’

Coordinate reference systems

- how to switch from PROJ.4 to PROJ.7 in R
- open session: questions from the participants
 
## Prerequisites

Attendees are expected to have a working recent version or R and RStudio installed, along with several R packages listed below.

### Required

```r
install.packages("remotes")
# select "2: CRAN packages only"
remotes::install_github("geocompr/geocompkg", 
                        upgrade = "ask", dependencies = TRUE, force = TRUE)
remotes::install_github("nowosad/spDataLarge")
```
