---
title: 'Lab 4'
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-29'
due: '2025-01-29'
slug: lab-4
categories:
  - Assignments
tags:
  - Labs
toc: true
---

## Overview
Because we will have a visitor today, this is a very short lab. The purpose of this lab is to help you to use color to your advantage. 
You will be asked to use a variety of color palettes, and use color for its three main purposes: 
(a) distinguish groups from each other, (b) represent data values, and (c)
highlight particular data points. Lab PS-3 will build on this lab that will also add an exporation of `themes`.

## Data

* We'll be working with the honey production data from #tidytuesday. [The #tidytuesday repo](https://github.com/rfordatascience/tidytuesday/tree/master/data/2018/2018-05-21) 
contains the full data, but we'll work with just the cleaned up version, using
the *honeyproduction.csv* file, which is posted in the data folder in the course repo.

## Lab Tasks

### Load Data

### Wrangle Data 

1. Visualize the total production of honey across years by state  Use color to
highlight the west coast (Washington, Oregon, and California) with a different color used for each west coast state.
  + **Hint 1**: I'm not asking for a specific kind of plot, just one that does the preceding. But if you're trying to visualize change over time, a bar chart is likely not going to be the best choice.
  + **Hint 2**: To get each state to be a different color you should either map state to color (for your layer that adds the west coast colors) or use the [gghighlight](https://yutannihilation.github.io/gghighlight/index.html) package.

2. Reproduce the plot according three different kinds of color blindness, as
well as a desaturated version. 

3. Reproduce the plot using a color blind safe palette. 

## Finishing up
When you have finished the above, upload your rendered pdf file to canvas.
