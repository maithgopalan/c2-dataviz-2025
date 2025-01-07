---
title: Accessing a bunch of Course Data (for use in labs)
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-08'
due: '2025-03-19'
slug: accessing-the-data
toc: true
categories:
  - Data
  - Data Visualization Competition
tags:
  - Data
  - Misc
---



The data we will be using for this course comes from USAFacts, who collated the data from various other sources. These data are not particularly granular. The smallest unit of analysis is schools, so you will have to think on a macro level about the types of questions you want to address. Full instructions to accessing the data are provided for you on canvas in the Files section (see [here](https://canvas.uoregon.edu/courses/192573/files?preview=12782218)). 

The purpose of this document is to walk you through a few files and discuss some of their properties. Let's start by looking at the available files.


```r
library(edld652)
list_datasets()
```

```
##  [1] "EDFacts_acgr_lea_2011_2019"                                
##  [2] "EDFacts_acgr_sch_2011_2019"                                
##  [3] "EDFacts_math_achievement_lea_2010_2019"                    
##  [4] "EDFacts_math_achievement_sch_2010_2019"                    
##  [5] "EDFacts_math_participation_lea_2013_2019"                  
##  [6] "EDFacts_math_participation_sch_2013_2019"                  
##  [7] "EDFacts_rla_achievement_lea_2010_2019"                     
##  [8] "EDFacts_rla_achievement_sch_2010_2019"                     
##  [9] "EDFacts_rla_participation_lea_2013_2019"                   
## [10] "EDFacts_rla_participation_sch_2013_2019"                   
## [11] "NCES_CCD_fiscal_district_2010"                             
## [12] "NCES_CCD_fiscal_district_2011"                             
## [13] "NCES_CCD_fiscal_district_2012"                             
## [14] "NCES_CCD_fiscal_district_2013"                             
## [15] "NCES_CCD_fiscal_district_2014"                             
## [16] "NCES_CCD_fiscal_district_2015"                             
## [17] "NCES_CCD_fiscal_district_2016"                             
## [18] "NCES_CCD_fiscal_district_2017"                             
## [19] "NCES_CCD_fiscal_district_2018"                             
## [20] "NCES_CCD_nonfiscal_district_2017_2021_directory"           
## [21] "NCES_CCD_nonfiscal_district_2017_2021_disabilities"        
## [22] "NCES_CCD_nonfiscal_district_2017_2021_english_learners"    
## [23] "NCES_CCD_nonfiscal_district_2017_2021_membership"          
## [24] "NCES_CCD_nonfiscal_district_2017_2021_staff"               
## [25] "NCES_CCD_nonfiscal_school_2017_2020_lunch_program"         
## [26] "NCES_CCD_nonfiscal_school_2017_2020_school_characteristics"
## [27] "NCES_CCD_nonfiscal_school_2017_2020_staff"                 
## [28] "NCES_CCD_nonfiscal_school_2017_2021_directory"             
## [29] "NCES_CCD_nonfiscal_school_2017_membership"                 
## [30] "NCES_CCD_nonfiscal_school_2018_membership"                 
## [31] "NCES_CCD_nonfiscal_school_2019_membership"                 
## [32] "NCES_CCD_nonfiscal_school_2020_membership"                 
## [33] "NCES_CCD_nonfiscal_state_2017_2020_directory"              
## [34] "NCES_CCD_nonfiscal_state_2017_2020_staff"                  
## [35] "NCES_CCD_nonfiscal_state_2017_2021_membership"
```

The names of these are not always super clear, and the variable names within the files are also regularly not straightforward. To start, anything that says `lea` is at the school district level, and anything that says `sch` or `school` is at the school level. 

## Data documentation
You can import any of these datasets and start to play around, but is **highly** encouraged that you also look at the corresponding documentation. Let's actually start by looking at the documentation for `"EDFacts_acgr_sch_2011_2019"`, which we know is at the school level, but otherwise it's pretty unclear.


```r
get_documentation("EDFacts_acgr_sch_2011_2019")
```

If you're on a Mac, the above code will download the documentation for this file and put it in a `data-documenation` directory (folder) inside your current working directory (your R project) and automatically open the file (in Microsoft Word in this case, but some documentation is also in Excel). Unfortunately, Windows machines make this process more difficult, so if you're on a Windows machine it will instead just print a link to the console that you can paste into your browser to get the documentation.

Scanning through this documentation we see that this file contains data (at the school level, given the file name) on the four-year adjusted-cohort graduation rates. According to the documentation, this is defined as

> The four-year adjusted-cohort graduation rate is the number of students who graduate in four years with a regular high school diploma divided by the number of students who formed the cohort for that graduating class. The four-year adjusted cohort rate also includes students who graduate in less than four years.

Section 1.6 is also important. It describes steps taken to ensure that individual students cannot be identified in the directory. This entails two steps:

* Cells with 1-5 students are suppressed. These are coded `PS`.
* Medium sized groups are binned (e.g. `"< 20%"`). The binning method depends on the size of the group. See Table 2 for more details.

## Getting the data
Let's go ahead and download the school district level version of this file, rather than schools, so it will be a bit quicker. Note that some of these datasets will take several minutes to download/import.


```r
grad_rates <- get_data("EDFacts_acgr_lea_2011_2019")
grad_rates
```

```
## # A tibble: 11,326 × 29
##    ALL_COHORT ALL_RATE CWD_COHORT CWD_RATE DATE_CUR ECD_COHORT ECD_RATE FIPST
##         <dbl> <chr>         <dbl> <chr>    <chr>         <dbl> <chr>    <chr>
##  1        252 80                3 PS       03OCT15         121 65-69    01   
##  2        398 75               47 70-79    03OCT15         233 65-69    01   
##  3       1020 89               51 40-49    03OCT15         175 75-79    01   
##  4        750 91               35 60-69    03OCT15         102 80-84    01   
##  5        128 55-59            15 LT50     03OCT15          68 40-44    01   
##  6        166 90-94             9 GE50     03OCT15          53 70-79    01   
##  7        336 90               30 60-79    03OCT15          35 60-69    01   
##  8        273 77               11 LT50     03OCT15          93 70-74    01   
##  9        134 70-74             4 PS       03OCT15          60 50-59    01   
## 10        266 58               33 50-59    03OCT15         195 55-59    01   
## # … with 11,316 more rows, and 21 more variables: FILEURL <chr>, LEAID <chr>,
## #   LEANM <chr>, LEP_COHORT <dbl>, LEP_RATE <chr>, MAM_COHORT <dbl>,
## #   MAM_RATE <chr>, MAS_COHORT <dbl>, MAS_RATE <chr>, MBL_COHORT <dbl>,
## #   MBL_RATE <chr>, MHI_COHORT <dbl>, MHI_RATE <chr>, MTR_COHORT <dbl>,
## #   MTR_RATE <chr>, MWH_COHORT <dbl>, MWH_RATE <chr>, STNAM <chr>, YEAR <dbl>,
## #   PIPELINE <chr>, DL_INGESTION_DATETIME <dttm>
```

## We will keep coming back to this data in future labs also! 