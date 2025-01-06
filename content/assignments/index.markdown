---
title: Assignments
toc: true
---


We will have 10 weekly in-class labs and three lab problem sets. The two will be very similar with two primary differences: (a) The labs will include designated time in class, though potentially not enough to complete the entire lab, and (b) all labs will be scored on a ["best honest effort"](../syllabus/#labs) basis, while lab problem sets will be scored based on accuracy. Note - all labs (in-class as well as the lab problem sets) may be completed independently or in small groups. I encourage the latter, and suggest working with the group you will be working with for your final project. However, all assignments completed as a group must use a shared GitHub repository.
Also, note that the weekly labs and slides will be uploaded to the class website the day before the weekly class (i.e., Tuesdays). You should make it a point to check and download those before coming to class.

#### A note on deadlines
I would like to, as much a possible, stick to the deadlines below so we can go over them together as a group *after* everyone has submitted their assignment. However, **if you need additional time for any reason** please just send me a note letting me know. You do not need to justify why. I would just ask that you not attend class during the time we are going over the assignment (but please attend the rest of the class if you are able).

## Lab Problem Sets

Each lab problem set is worth 20 points. Please do not turn in partial work. Instead, please ask for help and, if needed, an extension on the deadline. 

{{< bootstrap-table "table table-hover" >}}

| Lab Problem Set|Date Assigned   |Date Due         |Topic                                                                                     |
|---:|:---------------|:----------------|:-----------------------------------------------------------------------------------------|
|   1|Wed, January 8  |Mon, January 20  |[Collaborative git/GitHub, basic plots, and working with strings and text data](../lab-1) |
|   2|Wed, January 22 |Mon, Feb 3       |[Visual perception & reproducing plots](../lab-2)                                         |
|   3|Wed, February 05|Mon, February 17 |[Uses of color to enhance interpretability](../lab-3)                                     |

{{< /bootstrap-table >}}

## Final Project

The final project includes multiple components and is worth 70 points total (46% of your totalgrade), culminating in a data visualization portfolio. Your final project must be completed in groups of 2-3 and must include at least three data visualizations. You will build a web-deployed product (likely a dashboard or a website with blog posts) that not only displays the final visuals, but also clearly communicates the history of each visualization, how they evolved, and why you made the changes you did. You must use the [course data](../2021-12-10-accessing-the-data/index.html) for this project. The due dates for each component are as follows:

{{< bootstrap-table "table table-hover" >}}

|Component    |Date Due         | Points | Overall Grade Percentage|
|:------------|:----------------|:------:|------------------------:|
|Proposal     |Mon, January 27  |   20   |                     10 %|
|Presentation |Wed, March 12    |   20   |                     10 %|
|Product      |Wed, March 19    |   30   |                     15 %|

{{< /bootstrap-table >}}

The due date for the proposal can be (somewhat) flexible. However, unlike the lab problem sets, the remaining aspects of the final project cannot be changed and you will lose points if your work is submitted late without prior approval. This is mostly because of concerns related peer-review and completing the project by the end of the term.

### Proposal
The proposal process is a chance for you to get feedback  from me on your plans for the final project. The more information you provide me, the better feedback I will be able to provide you. The proposal is scored on a best honest effort basis. For full credit, please include each of the following:

* Research questions (probably 1-3)
* Preliminary ideas (even hand sketches) of different visualizations
* Some documentation that you have played with the course data some
* Names of the datasets you're thinking of using and what keys you'll need for joining the data
* Identification of the intended audience for each visualization 
  + Note, you might consider displaying the same data/relations more than 
    once, with each plot displayed for a different audience. If your group is planning on participating in the data visualization competition, you will need to plan for a broad general public audience for at least one of your visuals (it's okay if not all).
* The intended message to be communicated for each plot. 

### Peer Review
You will be assigned to three groups to review their code as part of an in-class lab session on Week 8. The purpose of this exercise is to learn from each other. Programming is an immensely open-ended enterprise and there are lots of winding paths that all ultimately end up at the same destination. In terms of visualization, there is certainly plenty of room for artistic license, but certain design decisions (as we will learn) can lead to more interpretable and better data communication. Peer review is a chance to learn from your peers both by reviewing their work and by having your work reviewed.

During your peer review, you must (at minimum) note the following:

* At least three areas of strength
* At least one thing you learned from reviewing their script
* at least one and no more than three areas for improvement **for each visualization**. 
* Comments on both the code leading up to (and including) the visualization, and the visualization itself (aesthetics, best practices, etc.).

Making your code publicly available can feel daunting. The purpose of this portion of the final project is to help us all learn from each other, not to denigrate. **Under no circumstances will overly harsh/negative comments be tolerated**. Any comments that could be perceived as overly critical and/or outside the scope of the code, will result in an immediate score of zero. 

Be constructive in your feedback. Be kind. We are all learning.


### Presentation
Week 10 will include each group sharing their portfolio with the class. If you opt-out of the data visualization competition, you will present early in the class period before the judges arrive. Those participating in the competition will present with the judges in attendance. Note that I hope to also invite others from the COE and will invite others from around the COE to attend as well.

I encourage you to present using HTML slides produced via R Markdown 
(specifically [xaringan](https://bookdown.org/yihui/rmarkdown/xaringan.html)), but this is not required. If you are interested in doing so but feel uncertain about the process, please get in touch with me and I can meet with you individually (or with a small group if there is sufficient interest) to help get you started. This is what I use for my course slides.

**Prior to the start of Week 10** please send me a link to your 
**published** presentation (not your repo, but your actual presentation).

You will likely have 10-12 minutes to share your portfolio, but the exact time allotment will depend on the number of groups. Please cover the following during your presentation:

* Briefly show each visualization
* Pick 1-2 to go more in-depth, and discuss
  + Intended audience
  + Design choices, e.g. 
    - Colors
    - Layout
    - Choice of specific type of plot
  + Prior version(s) and how the changes helped clarity, communication, beauty,
    etc.
  + At least 1 major challenge encountered along the way
  + At least 1 major victory

Note that I want to hear about your process as much as the final product. It is expected that not every piece of what you present is finalized. For example, if you are participating in the competition, you don't have to have each visual adhering to the USAFacts style guide at this point. However, you should be most of the way there and ready to share what you've produced.

### Product

The final project must include

* A web-deployed portfolio showcasing your [#dataviz](https://twitter.com/search?q=%23DataViz&src=tyah)
  skills using one of the following:
  + Website with [distill](https://rstudio.github.io/distill/),  
    [R Markdown](https://bookdown.org/yihui/rmarkdown/rmarkdown-site.html), or
    [blogdown](https://bookdown.org/yihui/blogdown/)
  + Technical document with [pagedown](https://github.com/rstudio/pagedown) or
    [bookdown](https://bookdown.org/yihui/bookdown/)
  + Scientific poster with [pagedown](https://github.com/rstudio/pagedown) or [posterdown](https://github.com/brentthorne/posterdown)
  + Data dashboard with [flexdashboard](https://rmarkdown.rstudio.com/flexdashboard/)
* At least four finalized data displays, with each accompanied by a strong narrative/story, **as well as the history** of how the visualization changed over time.

You must show iterations of your data displays, highlighting how 
they evolved over time and why you made the specific changes you did. If you go the website route, a blog post for each visualization showing their evolution would work great. Dashboards similarly have built in mechanisms to help show the history of plot.

The final project is required to be housed on GitHub and be fully reproducible. 
It will be graded on the following three criteria:

* At least four different visualizations (20 points; 5 points each)
  + Design choices (nothing violating the principles discussed in class)
  + Plot appropriate for given audience
  + Evolution of the plot is clear
* Reproducibility (5 points)
  + Should be housed on GitHub
  + I'll clone and try to reproduce - any differences between my local version and the published version will result in lost points
* Deployment (5 points)
  + Should be shareable via a link
  + No errors in the specific chosen format
  + Clear, clean, easy to follow/understand

## Extra Credit
There is one opportunity for extra credit, which is worth up to 10 
points. This includes an in-depth self-study of a topic not explicitly covered in the class. Students opting into the extra credit option will provide an (approximately) 10-20 minute presentation on their chosen topic to the class. For example, interactive and animated graphics are not explicitly covered, but packages like [gganimate](https://gganimate.com/index.html) and [plotly](https://plotly.com/r/) are powerful and fun. Network visualizations are also not covered but are nonetheless important. You could choose one of these areas, explore a different topic, or provide greater detail on a topic that *is* covered in class (e.g., geographic data). 

If you are interested in giving a talk on a topic of your choice, please contact me as soon as possible to obtain approval on the topic and set a date for the presentation.

