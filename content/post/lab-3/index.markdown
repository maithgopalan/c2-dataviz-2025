---
title: 'Lab 3'
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-22'
due: '2025-01-22'
slug: lab-3
categories:
  - Assignments
tags:
  - Labs
toc: true
---

## Overview

The purpose of this lab is to get you to try different methods of scale_*() options for visualizing the data and learn to explore what seems to work better. Specifically, you will work with changing colors, shapes, and sizes.

## Data 

You will use the `gapminder.csv` dataset. This is a cross-national dataset released by the World Bank’s Open Data portal. I have saved it in our class repo

## Tasks

### 1. Create a bar chart showing the number of distinct countries in each continent

Think carefully about how you are mapping the variables in the data to x, y, and fill to show in the bar chart

### 2. Use the discrete viridis color palette instead to see if this is better?  

### 3. Use arguments in the scale function, for instance, use the plasma palette from the viridis package as an option

### Would you change anything in the colors you see to improve he visualization? 

Hint: You can tell ggplot to not use the full range of the palette

### 4. Specify your own colors

Instead of letting R calculate the colors from a general palette, you can also specify your own colors with scale_fill_manual() and feeding it a list of values—generally as hex codes or a name from a list of built-in R colors

Hint: Use `scale_fill_manual()`


