---
title: "When should I quit research? An evidence-based approach"
author: "Adrian Barnett"
date: 2020-07-17
slug: quit-research
categories: []
tags: ['funding']
subtitle: ''
showtoc: false
image: "/img/path_5.jpg"
---

*Re-posted from [the AusHSI blog](https://www.aushsi.org.au/when-should-i-quit-research-an-evidence-based-approach/) (8 May 2015).*



After yet another failed fellowship application I considered if I should leave research. I now have seven fellowship failures and no successes, and that seems like a lot.

Success rates for grants are nose-diving and even the former head of the NHMRC says that [researchers should be considering other careers](https://www.theaustralian.com.au/higher-education/medical-phds-need-to-look-beyond-research-careers/news-story/f85cf01faa6a259d986395c7024dbf53) (pay-walled). I’ve spent a lot of time running research projects for no money, but working for no money is a luxury I can’t afford.

As a statistician I knew I could get a more objective answer of whether seven failures really is a lot. I used a Bayesian approach by creating a prior distribution of researchers and then adding my own data to get a posterior probability that I should quit. I decided I would quit if there was a more than 90% probability that I am in the bottom half of the talent pool. In other words, if there’s a high probability that I am below average.

My prior distribution aimed to capture the likely range in researcher quality. So I needed to think of the average researcher and the range in ability. If you think it’s a horrible idea to assign a number to researcher quality, then you should never apply for research funding. As a compromise we can call it the prior the distribution of researchers’ ability to write a good fellowship application, without opening the can of snakes of whether that’s actually well correlated with talent.

Here’s my prior:

<img src="/post/quit-research_files/figure-html/unnamed-chunk-1-1.png" width="70%" />

I wanted to have an average probability of success of 0.2, as that was about the average success of the schemes I had applied to. Then it’s logical to think of a few brilliant researchers, a few less than brilliant ones and most clumped around the mean. By trial and error I created the above prior, which is a Beta distribution (1,4), meaning that an average researcher would have 1 success and 5 attempts. If you understand this perfectly then you’re probably in the top half of the distribution.

Combining my data and the prior gives me this posterior:

<img src="/post/quit-research_files/figure-html/unnamed-chunk-2-1.png" width="70%" />

There is a 77% probability that I am in the bottom half, so I stay in research by a margin of 13% (I am this far from the 10% quit threshold). Sadly the evidence tells me that there’s an almost zero probability that I am a genius, and a relatively high probability that I am a plodder. Twelve failures are needed to reach the 90% margin, so the message for other people who have had multiple failures is: don’t give up hope yet.

Of course if (when) I do reach the 90% probability threshold then I’ll just move the goalposts to being 95% sure, which moves the failure threshold up to 16. Or if I do eventually quit research at least it will be a partly evidence-based decision.

If you want to run your own failure history, there's a shiny app [here](https://aushsi.shinyapps.io/quit/).
