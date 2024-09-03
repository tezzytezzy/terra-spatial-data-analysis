# Spatial Data Analysis with Terra

## Objective
Experimentation of spatial data analysis with terra in R.

Initially I used `library(raster)` but could not get data out via `getData("GADM", ...)`. The US Davies server that hosts the RDS file is well known to be flakey (documented [here](https://github.com/rspatial/raster/issues/169) and [here](https://github.com/rspatial/raster/issues/191)).  

## Installation
```
> sessionInfo()
R version 4.4.1 (2024-06-14 ucrt)
Platform: x86_64-w64-mingw32/x64
Running under: Windows 10 x64 (build 19045)

Matrix products: default


locale:
[1] LC_COLLATE=English_Canada.utf8  LC_CTYPE=English_Canada.utf8    LC_MONETARY=English_Canada.utf8 LC_NUMERIC=C                   
[5] LC_TIME=English_Canada.utf8    

time zone: America/Vancouver
tzcode source: internal

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] lubridate_1.9.3 forcats_1.0.0   stringr_1.5.1   dplyr_1.1.4     purrr_1.0.2     tidyr_1.3.1     tibble_3.2.1    ggplot2_3.5.1  
 [9] tidyverse_2.0.0 terra_1.7-78    readr_2.1.5    

loaded via a namespace (and not attached):
 [1] gtable_0.3.5      jsonlite_1.8.8    compiler_4.4.1    highr_0.11        tidyselect_1.2.1  Rcpp_1.0.13       jquerylib_0.1.4  
 [8] scales_1.3.0      yaml_2.3.10       fastmap_1.2.0     R6_2.5.1          generics_0.1.3    knitr_1.48        munsell_0.5.1    
[15] bslib_0.8.0       pillar_1.9.0      tzdb_0.4.0        rlang_1.1.4       utf8_1.2.4        stringi_1.8.4     cachem_1.1.0     
[22] xfun_0.46         sass_0.4.9        timechange_0.3.0  cli_3.6.3         withr_3.0.1       magrittr_2.0.3    digest_0.6.36    
[29] grid_4.4.1        rstudioapi_0.16.0 hms_1.1.3         lifecycle_1.0.4   vctrs_0.6.5       evaluate_0.24.0   glue_1.7.0       
[36] codetools_0.2-20  fansi_1.0.6       colorspace_2.1-1  rmarkdown_2.28    tools_4.4.1       pkgconfig_2.0.3   htmltools_0.5.8.1
> getRversion()
[1] ‘4.4.1’
```


## Dataset
[2011 Census - Boundary files by Statistics Canada](https://www12.statcan.gc.ca/census-recensement/2011/geo/bound-limit/bound-limit-2011-eng.cfm)  
[BC Gazetteer by BC Data Catalogue](https://catalogue.data.gov.bc.ca/dataset/d92224ee-03ef-4904-be53-b677d8e01ac4)  

## Reference
[Spatial Data Science](https://rspatial.org/)  
[Terra: Special Data Science](https://rdrr.io/cran/terra/)
