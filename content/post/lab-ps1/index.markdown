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
This lab covers three primary topics: (a) Working with R Markdown Files (b) working with downloading some education datasets using an API that's simpler than the one we did in the first class/lab!; and (3) extending the visualizations from Labs 2

## Data
You'll work with Urban Institute's [Education Data Portal](https://educationdata.urban.org/documentation/#r) which contains several education datasets and learn to download a relevant dataset

You'll also work with the combined births by day dataset used in Lab 2 to create a heatmap 

## Lab PS1 Tasks 

Glance through the data and the [repo](https://github.com/UrbanInstitute/education-data-package-r) that has excellent documentation. 

By the end, however, you should have:

* Initial explorations of the function `get_education_data` and the various available endpoints.

* Initial Explorations of `enrollment` through histograms

* A heat map of average births by day generated using the same `births` data we used in Lab 2

### 1. Install educationdata package and see what the endpoints are

### 2. Get Relevant Data 

Return a data.frame of `enrollment` across all grades for the most recent academic year for which the data is available from the Common Core of Data (just show head)  

### 3. Initial exploration
Create histograms and density plots of the `enrollment`. Try at least four different binning methods.

### 4. Re-load the combined `births` by day dataset used in Lab2 and generate a heatmap of average births by day 

* To do this, you need to make a summarized data frame with `group_by() |> summarize()` to calculate the average number of births by month and day of the month (i.e. average for January 1, January 2, etc.).

* You should then make a sort of calendar with date of the month on the x axis, month on the y axis, with heat map squares filled by the daily average. 

* Use geom_tile() to add squares for each day, and then add some extra scale, coordinates, and theme layers to clean up the plot

## Finishing up
When you have finished the above, upload your rendered (knit) HTML/pdf file to canvas.