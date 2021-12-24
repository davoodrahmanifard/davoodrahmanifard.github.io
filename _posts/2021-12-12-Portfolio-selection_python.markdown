---
layout: post
title: "Beginner's guid to portfolio selection with Python"
date: 2021-12-12 13:32:20 +0300
description: This is a short description how to make a portfolio by Python. # Add post description (optional)
img: PythonPort.jpg # Add image post (optional)
tags: [Python, Risk, Portfolio, Return] # add tag
---

## Introduction
Harry Markowitz introduced modern portfolio theory in his 1952 paper titled [Portfolio Selection] [Markowitz]. He begins by outlining that portfolio selection is a two-step process; firstly, an investor must consider the future performance of the available assets (in terms of both risk and return) and subsequently, a decision can be made about how to construct the portfolio (i.e. how much money to allocate to each asset).

The main objective of constructing a portfolio is to reduce risk without necessarily decreasing expected rate of return. From this, risk and return are the main characteristics of the portfolio, or any financial instrument for that matter. Therefore, optimizing a portfolio is maximizing overall return while minimizing the risk. It is a hard task to do considering the fact that risk and return are positively correlated, meaning that if risk is high, return is high as well.

### Return
Buying a financial asset can bring two types of return: dividend or interest payment and capital gain/loss. Therefore, return for the entire single holding period is as follows:

<img src="https://render.githubusercontent.com/render/math?math=R%20%3D%20capital%20gain%20%2B%20dividend%20yeild%20%3D%20%5Cfrac%7BP_%7Bt%7D-P_%7Bt-1%7D%2BD_%7Bt%7D%7D%7BP_%7Bt-1%7D%7D">

However, this calculation doesn’t take into account the length of the period, holding period could be a month or even 10 years. The fact that this return is not annualized makes it hard for us to use it for comparison.
For multiple periods, like several years, we can use either mean return or geometric mean return to aggregate the rates of return. Former one calculates overall return by dividing the sum of returns by the number of periods (years). Pretty easy and straightforward. However, this method assumes that the amount invested in the same at the beginning of each period, hence, it doesn’t take into account the compounding of return. This is why geometric mean return is a better representation of portfolio return.

Here we assume that our portfolio is a long-term “buy-hold” portfolio, therefore using geometric mean is more suitable. Please note that using historical returns for calculating expected returns (in our case calculating geometric mean of historical returns and using is as a proxy for expected return) could be inaccurate in some cases!

### Risk
Portfolio risk is a chance that the combination of assets or units, within the investments that you own, fail to meet financial objectives.
We calculate risk by measuring volatility of the returns using statistical measures such as variance, standard deviation, and covariance. Calculating standard deviation of a single financial asset is pretty straightforward: <img src="https://render.githubusercontent.com/render/math?math=%5Csigma%20%3D%20%5Csqrt%7B%5Cfrac%7B1%7D%7BN%7D%20%5Csum_%7Bi%3D1%7D%5EN%20(x_i%20-%20%5Cmu)%5E2%7D%20">.

But when it comes to finding the portfolio’s variance, weighted average of financial assets’ variances will not do the trick because we have to consider correlation between the assets. The general equation goes like this:
<img src="https://render.githubusercontent.com/render/math?math=%5Csigma%5E2%20%3D%20%20%5Csum_%7Bi%2Cj%3D1%7D%5EN%20%20%20w_%7Bi%7D%20w_%7Bj%7D%20Cov(R_%7Bi%7D%20R_%7Bj%7D)">
Note that in order to simplify the evaluation, we assume that the returns are normally distributed, therefore can be described by its mean and variance. If this assumption is violated, there would be additional characteristics such as skewness and kurtosis.

## Python codes



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

