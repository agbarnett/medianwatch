---
title: "Testing baseline tables in trials for signs of fraud"
author: "Adrian Barnett"
date: "2025-04-23"
draft: false
slug: baseline_testing
tags:
- fraud
- p-values
subtitle: ''
description: ''
showtoc: false
image: /img/duckboards_1.jpg
---

When fraudsters make up research data, they can make mistakes. Real data is rich and complex whilst fraudsters are on a get-rich-quick scheme and make slapdash errors. 

One mistake they make is in randomised trials, where it's standard to have a baseline table that compares the randomised groups. As the groups are randomised, the summary statistics should be similar. Fraudsters have no sense of 'similar' and so have created data where the groups are nearly identical. Others have gone too far the other way and created implausible differences between groups.

## Carlisle's test

The approach to testing baseline tables has been led by [John Carlisle](https://www.nature.com/articles/d41586-019-02241-z) and he has used his test to spot multiple fraudulent papers. His test uses the distribution of p-values for the between group differences and tests whether the p-values follow a uniform distribution, as they should under the null hypothesis that the groups were correctly randomised.

## A Bayesian test

I created an [alternative Bayesian test](https://f1000research.com/articles/11-783) that examines the symmetry of the t-statistics rather than the distribution of p-values. P-values are bounded between 0 to 1, which creates floor and ceiling effects. Bounded distributions are always harder to work with than unbounded. 

Carlisle's uniform test is also sensitive to false positives, for example where there's no between group differences but some of the [data are skewed data, or the summary statistics are rounded](https://doi.org/10.1371/journal.pone.0076010). 

A key advantage of my test is that it can deal with categorical as well as continuous data, whereas Carlisle's test can only use continuous data. This greatly increases the available data as over half the summary statistics in a sample of over 2,000 trials were percentages (see Table&nbsp;4 [here](https://f1000research.com/articles/11-783)).

Some authors have used Carlisle's test with categorical variables, but as pointed out by Daniel Tausk this creates [false positives](https://arxiv.org/abs/2209.00131). To illustrate the problem, Tausk simulated data from two groups of randomised patients with 100 patients per group with a binary variable that had a 5% chance of being "Yes". As shown in figure&nbsp;1 below, Fisher's exact test is conservative as it does not keep up with the ideal type&nbsp;1 error, whereas the t-test is almost perfectly on the ideal diagonal line. 

![Figure 1](https://github.com/agbarnett/medianwatch/raw/3c7a5b93f526f5282b0c9d72cc2a9b4c0b2f8d33/content/tausk_fig2.jpg)

#### Figure 1: Cumulative distribution functions for Fisher's exact p-value and a t-test versus the uniform distribution (diagonal line). 100 patients per group with a binary variable probability of "yes" of 0.05. The data were created with no difference between the randomised groups. 

The ability of the t-test to deal with categorical data was shown by [D'Agostino and colleagues](https://www.tandfonline.com/doi/abs/10.1080/00031305.1988.10475563) back in 1988, who showed that the independent samples t-test beats Fisher's exact test and the Chi-squared test for 2$\times$2 categorical data. This will be a surprise to the "statistics by recipe" crowd, who insist on choosing tests using flow charts and/or dogma.

As the Fisher's exact test p-values deviate from the uniform distribution, then using Carlisle's test will lead to an excess of false positives when the null hypothesis is true. This is shown in Figure&nbsp;2 (again reproducing Tausk's paper) for simulated data with 20 categorical variables each with a 0.5 chance of being "Yes". As before, there are two groups with 100 patients per group. 

![Figure 2](https://github.com/agbarnett/medianwatch/raw/3c7a5b93f526f5282b0c9d72cc2a9b4c0b2f8d33/content/tausk_fig6.jpg)

#### Figure 2: Cumulative distributions for Stouffer's test for uniform p-values and my Bayesian test for illustration. 100 patients per group, 20 binomial variables, and probability of "yes" equal to 0.5. The data were created with no difference between the randomised groups. 

I've added my Bayesian test to Figure&nbsp;2, but the posterior probability from a Bayesian test does not behave like a standard p-value. However, the plot still shows that the Bayesian test often gives a low posterior probability when the null hypothesis is true, which is useful. 

My test is available [online here](https://aimos.shinyapps.io/baseline/) and for papers on _PubMed Central_, there's some automated code that tries to extract the baseline table.
