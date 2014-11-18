---
title       : Mpg versus AM
subtitle    : An easy attempt to choose a car
author      : ClaudioI
job         : Coursera student
logo        : loype.png
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Summary

This short presentation aims at describing the Shiny Application I made as a project for 
the Coursera **Developing Data Products** course.


The Project Assignment states: " get 5 slides (inclusive of the title slide) to pitch your App."

My App produces some plots using the `mtcars`, a famous dataset included in the Package `datasets`. 

The idea of using  `mtcars` relates with a previuos Coursera course: Regression Models.
In this course I was asked to make a project responding to "*Is an automatic or manual transmission better for MPG*"

The result of the Regression Course project is not here. You can bet your solution.



--- .class #id 

## Background


The data, included in  `mtcars`, was extracted from the 1974 Motor Trend US magazine, and comprises fuel consumption and 10 aspects of automobile design and performance for 32 automobiles (1973-74 models).

The first records of the dataset are:


```
##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1
```

The `mpg` has a quite normal distribution. In `am` automatic occurs 19, manual 13.

--- .class #id 

## Apps description

The App is made of two panels:

`About` where you could find a basic documentation of what the app is about.  

`Plot` where you could choose between three different Scatterplot. Each one shows how `mpg` is related with three key predictors available in the dataset.


--- .class #id 

## Scatterplot operation 


Please select a variable to be shown in relationship with `mpg`:

- `wt` Weight in lb/1000

- `disp` Displacement in cu.in.

- `hp` Gross horsepower

The different shape of the points outlines the number of cylinders; the colour of the points says the transmission type .

You can choose if you want to  show also the trend line.

The three scatterplots suggest how `mpg` is related with `am`.



