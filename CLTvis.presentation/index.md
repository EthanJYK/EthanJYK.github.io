---
title       : "Central Limit Theorem Visualisation"
subtitle    : (Use Arrow Keys to Flip Pages)
author      : "Junyoung Kim"
job         : "September 9, 2018"
framework   : io2012       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---


## Introduction

- [Central Limit Theorem](https://en.wikipedia.org/wiki/Central_limit_theorem) is a key concept in the frequentist probability theory: **Even if the original distribution is not normally distributed, the distribution of its sample means tends toward a normal distribution.** The idea itself is very simple, but it is somewhat hard to grasp for statistics learners only with written words and formulas. 

- My web-application, [Central Limit Theorem Visualisation](https://ethanjyk.shinyapps.io/cltvis/) shows how central limit theorem works by rendering how plots change as the number of sample means increases. And, it is **SUPER EASY**. 

  - Choose a distribution
  - Adjust shapes
  - Click buttons to add sample means
  - ... **PROFIT!!**

--- 

## Let's See How It Works

- Here is the overall layout of the app.

<img style="float: left;" src="0.png", width=686, height = 495> 

---

## Let's See How It Works: Main Plot panel

- You can see the **Main Plot** panel on the top left.

<img style="float: left;" src="1.png", width=267, height = 446> <br></br>

&nbsp;&nbsp;&nbsp;&nbsp;- Choose a Distribution Type to create a pool of numbers.

&nbsp;&nbsp;&nbsp;&nbsp;- Move slider to adjust skewness.

&nbsp;&nbsp;&nbsp;&nbsp;- Below "Skewness" slider... 

&nbsp;&nbsp;&nbsp;&nbsp;- The panel shows the mean(mu) and standard deviation(sigma).


---

## Let's See How It Works: Main Plot panel

- **Main Plot** panel and the plot created using input values.

<img style="float: left;" src="2.png", width=750, height = 400>


---

## Let's See How It Works: Sample Mean Plot panel

- You can also see the **Sample Mean Plot** panel on the bottom left.

<img style="float: left;" src="3.png", width=267, height = 487> <br></br>

&nbsp;&nbsp;&nbsp;&nbsp;- Move slider to adjust the size of each sample(N) out of your pool.

&nbsp;&nbsp;&nbsp;&nbsp;- Click 5 / 100 Button to put additional sample means to the plot.

&nbsp;&nbsp;&nbsp;&nbsp;- Click more and see how the sample mean plot changes. 

&nbsp;&nbsp;&nbsp;&nbsp;- The plot approximates normal as the number increases.


---

## Let's See How It Works: Sample Mean Plot panel

- **Sample Mean Plot** panel and the plot created using input values.

<img style="float: left;" src="4.png", width=750, height = 400>


---

## Let's See How It Works: Comparing Results

- Compare means and standard deviations of two plots.

<img style="float: left;" src="5.png", width=315, height = 511> <br></br>

&nbsp;&nbsp;&nbsp;&nbsp;- With the number of sample means large enough(ex = 9900),

&nbsp;&nbsp;&nbsp;&nbsp;- the mean of your sample means becomes closer to the μ.

&nbsp;&nbsp;&nbsp;&nbsp;- and their standard deviation approximates sigma/sqrt(N), 

&nbsp;&nbsp;&nbsp;&nbsp;- 0.1167 / sqrt(25) = 0.02334 .... very close to 0.02295

&nbsp;&nbsp;&nbsp;&nbsp;- **The reality works just as the formula says!**

---

## Links

- [Central Limit Theorem Visualisation](https://ethanjyk.shinyapps.io/cltvis/)

- You can also see the source codes on [my github repository](https://github.com/EthanJYK/datasciencecoursera/tree/master/9.%20Developing%20Data%20Products/CLTvis). 