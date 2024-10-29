---
layout: post
title: Data analysis resources
date: 2019-02-01
categories: open-science
tag: resources
---

Most of my current data analysis uses R and R packages. During college, I first used proprietary programs for statistical analysis. The learning curve was not so steep, but replicating the analyses became difficult after changing computers or losing access to the software licences (They were quite expensive for a student!). Additionally, using these programs became more difficult when I changed my operating system to a [GNU/Linux](https://www.gnu.org/) distribution that was more according to my [philosophy](https://www.gnu.org/philosophy/philosophy.html).

​I finally decided to stop being scared of R and tried it during my first year in grad school. Yes, it took me more time to learn how to start using it, but now I cannot go back to any other software for my statistical analyses and graphics. R has thousands of packages, so you have almost limitless options.

R also makes it easier to do reproducible and open science. It is free, runs on UNIX, Windows and MacOS, and if you are good keeping scripts that are well documented and organized, anyone could reproduce and validate your analyses! I personally like the R (for statistics and graphics), Markdown (for nice code documentation), git (for version control) and GitHub (for hosting/sharing/collaboration) combo.   

I found that learning R and the nuances of its packages was easier when I was running my own analysis. I suggest to get familiar with the basics and then jump into your own work even if it seems complicated.

​
Here are some useful links and materials to get started: 

**R**:

* [R manuals](https://cran.r-project.org/doc/contrib/) in multiple languages

* R studio offers a graphical user interface  

* [R packages](https://r-pkgs.org/) will help you to develop good R coding practices. Also has a chapter on using [RStudio, Git and GitHub together](https://r-pkgs.org/git.html#git-rstudio). 

​
**Git and GitHub**:

* [Pro Git](https://git-scm.com/book/en/v2) book by Scott Chacon and Ben Straub. I followed this step by step when I was learning to use git. Highly recommended

* [Ten Simple Rules for Taking Advantage of Git and GitHub](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947)

​
**Markdown**:

* Markdown [Cheat Sheet](https://www.markdownguide.org/cheat-sheet)

* [R Markdown](https://rmarkdown.rstudio.com/)


**Integration**:

* R and git: Using Git with RStudio

* Markdown and GitHub​ (Writing on GitHub)

<br>

This is an **example** of data analysis in which I integrated these tools to make the project reproducible: 
​
Data analysis for the paper [*Coral reef resilience to thermal stress in the Eastern Tropical Pacific*](doi:10.1111/gcb.15126)

* GitHub [repository](https://github.com/anampc/ETP_reef_resilience) with R scripts, data, and ReadMe file

* Repository [output](http://anampc.github.io/ETP_reef_resilience/) generated with Markdown and Knit

* Repository [archive](https://zenodo.org/record/3744864) in Zenodo that corresponds with the last version of the data published​
