---
layout: post
title: "Beginner's guid to portfolio selection with Python"
date: 2021-12-12 13:32:20 +0300
description: This is a short description how to make a portfolio by Python. # Add post description (optional)
img: PythonPort.jpg # Add image post (optional)
tags: [C++, Optimization, Portfolio, Genetic Algorithms] # add tag
---

## Introduction
Harry Markowitz introduced modern portfolio theory in his 1952 paper titled [Portfolio Selection] [Markowitz]. He begins by outlining that portfolio selection is a two-step process; firstly, an investor must consider the future performance of the available assets (in terms of both risk and return) and subsequently, a decision can be made about how to construct the portfolio (i.e. how much money to allocate to each asset).

Essentially, portfolio is a grouping of financial assets such as stocks, bonds, commodities, cash equivalents and others. Now the million-dollar-question is “How much of what should my portfolio consist of?” The main objective of constructing a portfolio is to reduce risk without necessarily decreasing expected rate of return.
From this, risk and return are the main characteristics of the portfolio, or any financial instrument for that matter. Therefore, optimizing a portfolio is maximizing overall return while minimizing the risk. It is a hard task to do considering the fact that risk and return are positively correlated, meaning that if risk is high, return is high as well.

### Return
Buying a financial asset can bring two types of return: dividend or interest payment and capital gain/loss. Therefore, return for the entire single holding period is as follows:



The selection of optimal portfolios is the central problem of financial investment decisions. Mathematically speaking, portfolio selection refers to the formulation of an objective function that determines the weights of the portfolio invested in each asset as to maximize return and minimize risk.

This study presents the development of a system, based on Genetic Algorithm, in the process of the selection of portfolio and determination of the percentages to be invested in each asset, called the weight of the aaset in the investment portfolio management.The objective of the work is to evaluate the performance of Genetic Algorithms for portfolio selection and optimization. Portfolio selection and optimization are problems of multiple objectives (risk, return and correlation) where it is desired to choose a set of actions of companies with profit perspective to form an investment portfolio.

>This model does not have any limitation as far as the number of assets, is concerned.Parameters that affect the time of running the program in addition to the memory and CPU of the computer are number of assets and size of the population in each generation.

This study developed in 3 main steps:
* a study on portfolio selection and optimization and Genetic Algorithms literature
* design two appropriate Genetic Algorithms for two mathematical models which designate the appropriate portfolios and their optimal weights
* compare this method with linear and quadratic portfolio modeling for small scale problems and apply the designed models for a large scale real case of Alborz Insurance Company.


Check out the [full text][full-doc] for more info and the [codes][codes-repo] written in C++ on my Github repo.

[Markowitz]: https://www.math.hkust.edu.hk/~maykwok/courses/ma362/07F/markowitz_JF.pdf
[codes-repo]:   https://github.com/davoodrahmanifard/GA-for-Portfolio-Selection

