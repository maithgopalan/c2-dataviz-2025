---
title: 'Lab 2'
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-15'
due: '2025-01-15'
slug: lab-2
categories:
  - Assignments
tags:
  - Labs
toc: true
---

## Overview
The purpose of this lab is to get you to try different methods of visualizing the same data to explore what seems to work better.

## Data

* We’ll use data from the CDC and the Social Security Administration about the number of daily births in the United States from 1994–2014 to do get more familiar with ggplot

* FiveThirtyEight reported a [story](https://fivethirtyeight.com/features/some-people-are-too-superstitious-to-have-a-baby-on-friday-the-13th/) using this data in 2016 and they posted CSV files on [GitHub] (https://github.com/fivethirtyeight/data/tree/master/births), so we can download and use those (also saved the csv files on class repo if you want to pull from there)

## Lab Tasks

# Load Data

There are two CSV files:

`US_births_1994-2003_CDC_NCHS.csv` contains U.S. births data for the years 1994 to 2003, as provided by the Centers for Disease Control and Prevention’s National Center for Health Statistics.

`US_births_2000-2014_SSA.csv` contains U.S. births data for the years 2000 to 2014, as provided by the Social Security Administration.
Since the two datasets overlap in 2000–2003, we use Social Security Administration data for those years.

You can downloaded the data from GitHub or from the class repo. You’ll then load them with read_csv() and combine them into one data frame.

# Wrangle Data 

Start with looking at the first few rows of the data to see what we’re working with

* You will notice that the columns for year and births seem straightforward and ready to use. 

* The columns for month and day of the week could be improved if we changed them to text (i.e. January instead of 1; Tuesday instead of 3).

# To fix this, convert these columns to categorical variables, or factors in R. 

* Hint 1 - You can use c() function to make a list of values for both months and day names

* Hint 2 - You can then make month and days as ordered factors using rhe labels

# Make Bar Plot of Total births by Weekdays

# Learn to play with the fill color to highlight the most salient trends  

# Use one (or two other) type(s) of plot we learned in class today on this data that you think will be appropriate  

## Finishing up
When you have finished the above, upload your R code/rendered (knit) HTML/pdf file to canvas.
