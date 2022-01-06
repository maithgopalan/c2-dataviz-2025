---
title: Schedule
toc: true
---




<div class="sds-book">

[Social Data Science with R](https://www.sds.pub)
* Daniel Anderson
* Brendan Cullen
* Ouafaa Hmaddi

</div>

In addition to the course books linked below, I started working on course notes for all of the classes last year. This may eventually turn into a published book, but for now I'm just thinking of it as course notes. It has also mostly stalled in its development because of perpetual competing demands. Please feel free to use these notes as a supplemental resource (in addition to the slides and lectures). Also, please let me know if you'd like to contribute! In particular, if you see typos or areas that are unclear, that feedback would be really helpful. You can fork the repo and submit a PR and be a contributor to the book!

## Course Books
Each of the below links to the full book. Icons in the schedule link to specific chapters. Note that occasionally are external resources that I will ask you to complete that are not readings (i.e., there are two videos it would be helpful if you watched).

{{< course-books >}}


 ## Week 1 
 {{< schedule >}}

{{< week-odd "01-03" >}}
  {{< description "Introduction to the course and accessing course data" "Introductions and the weekly schedule of topics. I'll briefly talk about git and plead with you to watch last year's lecture and read on git workflows (we won't have time to cover it this year; MLK week might be a good time for this). We'll then spend the rest of the day working on (a) connecting to a remote course data repository, and (b) making queries to get the data you want." >}}
  {{< wrap >}}
{{< slides "w1" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< assigned "syllabus/#final-project" "Final" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< readings "video" "https://www.youtube.com/watch?v=X7Cl3lwxXi4" "" >}}
{{< readings "other" "https://www.sds.pub/collaborating-with-git-and-github.html" "8" >}}
{{< readings "happygit" "git-branches.html" "22" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "https://youtu.be/CeobEaNT0Mo" >}}
{{< /wrap >}}
{{< /week-odd >}}

{{< /schedule >}}
 ## Week 2 
 {{< schedule >}}

{{< week-even "01-10" >}}
  {{< description "Intro to visualizations and working with string data, & Lab 1" "We will look at different types of visualizations with a specific focus on continuous variables. We will explore how different choices with these visualizations can change your inferences. We will then move to string data more specifically and methods for quickly visualizing a corpus . We will then practice these topics with our first lab." >}}
  {{< wrap >}}
{{< slides "w2" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< assigned "lab-1" "Lab 1" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< readings "socviz" "groupfacettx.html#groupfacettx" "22" >}}
{{< readings "r4ds" "graphics-for-communication.html" "4" >}}
{{< readings "r4ds" "strings.html" "14" >}}
{{< readings "dataviz" "directory-of-visualizations.html" "28" >}}
{{< readings "dataviz" "visualizing-amounts.html" "6" >}}
{{< readings "socviz" "gettingstarted.html#gettingstarted" "5" >}}
{{< readings "socvi" "makeplot.html#makeplot" "7" >}}
{{< readings "other" "https://www.tidytextmining.com/tidytext.html" "1" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-even >}}

{{< /schedule >}}
 ## Week 3 
 {{< schedule >}}

{{< week-odd "01-17" >}}
  {{< description "Martin Luther King Jr. Day" "No class. Black Lives Matter. ![](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.pngmart.com%2Ffiles%2F13%2FBlack-Lives-Matter-Fist-Transparent-PNG.png&f=1&nofb=1)" >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< due "lab-1" "Lab 1" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "NA" "NA" "NA" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-odd >}}

{{< /schedule >}}
 ## Week 4 
 {{< schedule >}}

{{< week-even "01-24" >}}
  {{< description "Visual Perception & Lab 2" "Aesthetic mappings and visual encodings of data. The data-ink ratio and the pitfall of rigid rules. Some general rule of thumb recommendations. For the lab, we will use ggplot2 to replicate plots produced by [fivethirtyeight](https://fivethirtyeight.com)." >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< assigned "lab-2" "Lab 2" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< due "assignments/#proposal" "Prop" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "socviz" "lookatdata.html#lookatdata" "1" >}}
{{< readings "dataviz" "aesthetic-mapping.html" "2" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-even >}}

{{< /schedule >}}
 ## Week 5 
 {{< schedule >}}

{{< week-odd "01-31" >}}
  {{< description "Color & Lab 3" "Three primary means by which color can aid interpretation. Color blindness considerations and color palettes that work well. Common pitfalls with the use of color. We will use color for each of its primary uses in data visualization and explore and evaluate different palettes by different types of color blindness." >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< assigned "lab-3" "Lab 3" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< due "lab-2" "Lab 2" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "dataviz" "color-basics.html" "4" >}}
{{< readings "dataviz" "color-pitfalls.html" "19" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-odd >}}

{{< /schedule >}}
 ## Week 6 
 {{< schedule >}}

{{< week-even "02-07" >}}
  {{< description "Communication & Intro to uncertainty" "Refining your plots for communication. We'll discuss annotating plots, aspect ratios, scales, and a bit on theming. Common methods for visualizing uncertainty (and their implementation w/{ggplot2}). Framing uncertainty as relative frequencies. Non-standard methods for visualizing standard errors, boostrapping, and a brief foray into hypothetical outcomes plots" >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< assigned "homework-1" "HW 1" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< due "lab-3" "Lab 3" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "socviz" "refineplots.html#refineplots" "8" >}}
{{< readings "dataviz" "redundant-coding.html" "20" >}}
{{< readings "dataviz" "balance-data-context.html" "23" >}}
{{< readings "dataviz" "telling-a-story.html" "29" >}}
{{< readings "dataviz" "visualizing-uncertainty.html" "16" >}}
{{< readings "video" "https://www.youtube.com/watch?v=E1kSnWvqCw0&feature=youtu.be" "" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-even >}}

{{< /schedule >}}
 ## Week 7 
 {{< schedule >}}

{{< week-odd "02-14" >}}
  {{< description "Finishing up uncertainty & intro to tables and fonts" "We will focus primarily on two packages for creating tables: [{gt}](https://gt.rstudio.com) for static tables, and [{reactable}](https://glin.github.io/reactable/index.html) for interactive tables. We'll also discuss changing fonts, both within websites/applications, as well as with {ggplot2}." >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< readings "socviz" "workgeoms.html#workgeoms" "5" >}}
{{< readings "other" "https://gt.rstudio.com/articles/intro-creating-gt-tables.html" "gt" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-odd >}}

{{< /schedule >}}
 ## Week 8 
 {{< schedule >}}

{{< week-even "02-21" >}}
  {{< description "Websites, flex dashbaords, and some customization with CSS" "Building (static) data dashboards with the [{flexdashboard}](https://rmarkdown.rstudio.com/flexdashboard/) package. We'll discuss layouts, including multi-page layouts, storyboards, icons, and publishing through GitHub." >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< assigned "assignments/#peer-review" "PR" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< due "assignments/#draft" "Draft" >}}
{{< due "homework-2" "HW2" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "other" "https://rstudio.github.io/distill/" "distill" >}}
{{< readings "other" "https://bookdown.org/yihui/rmarkdown/websites.html" "sites" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-even >}}

{{< /schedule >}}
 ## Week 9 
 {{< schedule >}}

{{< week-odd "02-28" >}}
  {{< description "Intro to Geographic data" "Understanding the difference between vector and raster data, producing basic maps, getting data for producing different types of maps, and understandin the basics of the R geospatial ecosystem (which is consistently and rapidly evolving)." >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< due "assignments/#peer-review" "PR" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "socviz" "maps.html#maps" "7" >}}
{{< readings "dataviz" "geospatial-data.html" "15" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-odd >}}

{{< /schedule >}}
 ## Week 10 
 {{< schedule >}}

{{< week-even "03-07" >}}
  {{< description "Loose ends and presentations" "We cover a lot in this course and so there is some space here to dive deeper into topics we didn't cover thouroughly enough, or additional topics as suggested by you and your peers. Each group will also present on their data visualization portfolios and discuss their journey, including high points and challenges faced along the way." >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< readings "NA" "NA" "NA" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-even >}}

{{< /schedule >}}
 ## Week 11 
 {{< schedule >}}

{{< week-odd "03-14" >}}
  {{< description "Finals Week" "Your final project is due before midnight" >}}
  {{< wrap >}}
{{< slides "" >}}
{{< /wrap >}}
  {{< wrap >}}

{{< /wrap >}}
  {{< wrap >}}
{{< due "assignments/#final-project" "Product" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< readings "NA" "NA" "NA" >}}
{{< /wrap >}}
  {{< wrap >}}
{{< lecture "" >}}
{{< /wrap >}}
{{< /week-odd >}}

{{< /schedule >}}

