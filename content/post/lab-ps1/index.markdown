---
title: Lab Problem Set 1
author: Maithreyi Gopalan
date: '2025-01-06'
assigned: '2025-01-08'
due: '2025-01-20'
slug: lab-ps1
categories:
  - Assignments
tags:
  - Labs
toc: true
---



## Overview
This lab covers three primary topics: (a) working with *git* and *GitHub*
  collaboratively, (b) creating basic visualizations, and (c) working with textual data.You should plan to work together with your group.

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
We'll work with Week 1 of the [#tidytuesday](https://twitter.com/search?q=%23tidytuesday&src=tyah)  data for 2019, specifically the [#rstats](https://twitter.com/search?q=%23rstats&src=typd) dataset, containing nearly 500,000 tweets over a little more than a decade using that hashtag. The data is in the `data` folder of the course repo.

## Project

Glance through the plots below. This is an open-ended lab. You need to work with your group to figure out how to best approach this. By the end, however, you should have:

* A shared GitHub repo

* Initial explorations of the `display_text_width` variable, including different binning methods.

* Final versions of each of the two plots

* At least two branches, each of which have been merged in


Each person should be responsible for **at least** one commit. 




### 1. Initial exploration
Create histograms and density plots of the `display_text_width`. Try at least four different binning methods and select what you think best represents the data for each. Provide a brief justification for your decision.




### 2. Look for "plot"
Search the `text` column for the work "plot". Report the proportion of posts containing this word.




### 3. Plot rough draft
Create the following figure of the 15 most common words represented in the posts.

<img src="{{< blogdown/postref >}}lab-ps1/index_files/figure-html/fig2-raw-1.png" width="960" />


#### Some guidance

* You'll need to drop a few additional words beyond stop words to get a clear picture as above. Consider removing rows where the word is not `%in% c("t.co", "https", "http", "rt", "rstats")`. This can be a bit tricky (see [here](https://stackoverflow.com/a/9852867/4959854) for additional help)

### 4. Stylized Plot
Style the plot so it (mostly) matches the below. It does not need to be exact, but it should be close.

<img src="{{< blogdown/postref >}}lab-ps1/index_files/figure-html/fig2-styled-1.png" width="960" />


## Finishing up
It is expected that this lab will take you more time than we will devote to it in class. Class time should be used to clarify any points of confusion and if you run into issues after class, please get in touch with me so we can arrange a time to meet and I can help you.

Once you have finished, please go to Canvas and submit a link to your shared repo. Credit will be awarded based on the commit history.
