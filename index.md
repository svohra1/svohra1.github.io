---
title       : Data Products Course Project - Slidify
subtitle    : CarPaymentCalc Shiny App
author      : SVohra
job         : Data Science Specialization Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## What?

1. An app that helps you compute your car payments
2. Just a simple webpage
3. Enter 4 pieces of information, and you're set

--- .class #id 

## Who?

1. It's for everyone and anyone
2. Targetted at those who are in the market for an automobile
3. People who might feel intimidated when negotiating financing options

---

## Why?

1. Gives the buyer more information about the purchasing process
2. Calculate your affordabily before going to the dealer
3. Understand the numbers behind the dealer's offer
4. It's FREE

---

## Example

1. Sale Price = $25000 and Downpayment = $2000
2. Interest Rate = 5% and Repayment Period = 7 years

```r
price <- 25000; downpayment<- 2000
rate <- 5; period <- 7
p <- price - downpayment
i <- (rate / 100) / 12
n <- period * 12
monthlyPayment <- (p * i) / (1 - (i + 1)^(-n))
monthlyPayment
```

```
## [1] 325.1
```
Simple and Easy!


