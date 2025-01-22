---
title: 'Lab Problem Set 2'
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-22'
due: '2025-02-03'
slug: lab-ps2
categories:
  - Assignments
tags:
  - Labs
toc: true
---

## Overview

The purpose of this lab is to get you more familiar with scale_*() options for visualizing the data and learn to explore what seems to work better. Specifically, you will work with changing colors, shapes, and sizes.

## Data 

You will use the same `gapminder.csv` dataset we used in Lab 3. 

## Tasks

# You got to work primarily just with color in lab 3. But scale functions also work for other aesthetics like shape or size. To see that, create a scatter plot with just one year 

## x mapped to gdpPercap
## y mapped to lifeExp 
## color and shape mapped to continent and
## size mapped to pop
## Show x-axis scale to be shown in log-scale (Hint: use scale_x_log10) 

# Change colors and shapes of the point 

Hint 1: Use `scale_color_*()` and with `scale_shape_*()`
Hint 2: If you run `?pch` in your console or search for `pch` in the help, you will see possible shapes

# Try changing the size next 

# Finally, If you load the {scales} library (which is installed as part of {tidyverse} but isn’t automatically loaded), you can use some neat helper functions to reformat the text that shows up in plots. For instance, we can make it so population is formatted as a number with commas every 3 numbers, and the x-axis is formatted as dollars. Try that.