---
title: Lab Problem Set 1
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-15'
due: '2025-01-27'
slug: lab-ps1
categories:
  - Assignments
tags:
  - Labs
toc: true
---



## Overview
This lab covers three primary topics: (a) working with *git* and *GitHub*
  collaboratively, (b) creating basic visualizations, and (c) working with some education datasets.You should plan to work together with your group.

The basics of the lab are to:
  
* Create a shared repo
* Create an R Markdown document
* Work on different pieces of the lab together
+ File issues for the different pieces of the lab
+ Create branches for those issues
+ Different people work on different branches - merge them in when you're ready
* Submit a link to the repo through Canvas when you've completed the lab
* I check the commit history, and give each person credit

To receive full credit **you must** create and merge branches. The contributions across team members should also appear roughly equal.

## Data
We'll work with Urban Institute's [Education Data Portal](https://educationdata.urban.org/documentation/#r) which contains several education datasets. 

## Project

Glance through the data and the [repo](https://github.com/UrbanInstitute/education-data-package-r) that has excellent documentation. This is an open-ended lab. You need to work with your group to figure out how to best approach this. By the end, however, you should have:

* A shared GitHub repo

* Initial explorations of the function `get_education_data` and the various available endpoints.

* Return a data.frame of `enrollment` across all grades for the most recent academic year for which the data is available from the Common Core of Data  

* Initial Explorations of `enrollment`

* At least two branches, each of which have been merged in


Each person should be responsible for **at least** one commit. 

### 1 Get Relevant Data 


### 2. Initial exploration
Create histograms and density plots of the `enrollment`. Try at least four different binning methods and select what you think best represents the data for each. Provide a brief justification for your decision.


### 3. Plot rough draft
Create the following figure of the 15 most common words represented in the posts.

<img src="../lab-ps1/index_files/figure-html/fig2-raw-1.png" width="960" />


### 4. Stylized Plot
Style the plot so it (mostly) matches the below. It does not need to be exact, but it should be close.

<img src="{{< blogdown/postref >}}lab-ps1/index_files/figure-html/fig2-styled-1.png" width="960" />


## Finishing up

Once you have finished, please go to Canvas and submit a link to your shared repo. Credit will be awarded based on the commit history.
