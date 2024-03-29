---
title: Dear p-values, it's not me, it's not you, it's everyone else
author: Adrian Barnett
date: '2020-09-08'
tags:
  - p-values
  - statistics
slug: pvalue_pledge
showtoc: no
image: /img/rail_1.jpg
bibliography: bibliography.bib
link-citations: yes
---

## Yet another p-value run-in.

For a recent observational study I tried to limit the use of p-values in the paper.
My colleagues wanted more p-values and I had to politely push back.
During one team meeting I even offered to put the p-values in if someone could accurately tell me what they meant … silence.

Predicting that the reviewers would also want to see more p-values, I added this sentence to the paper’s methods: “We have tried to limit the use of p-values, as they are often misunderstood or misinterpreted, and elected to discuss clinically meaningful differences.” Followed by a citation to Steve Goodman’s excellent “dirty dozen” paper on p-values ([Goodman 2008](#ref-Goodman2008)).

The Statistical Editor didn’t like my sentence and said (sic): “The authors should compare the various groups and report p-values. The readership of the AJRCCM is experience enough to not misunderstand.”

The journal rejected our paper, so feel free to interpret what follows as sour grapes.

## Do AJRCCM authors understand p-values?

It’s not easy to check the understanding of [AJRCCM](https://www.atsjournals.org/journal/ajrccm) readers, but I can easily check the understanding of AJRCCM authors.

I went to the journal’s current issue, looked at research papers, and did a search for “significan” to capture “significance” and “significant”. After looking at just three papers I found two clangers.

1.  From [this paper](https://www.atsjournals.org/doi/full/10.1164/rccm.201908-1546OC): “A randomly selected subset of 20 of the 54 samples were, however, regraded by the pathologist in a blinded fashion, resulting in a similarly statistically significant reduction of the goblet cell hyperplasia score (P=0.0013, data not shown).”

What’s wrong with this? There’s no mention of the size of the difference, so in Steve Goodman’s dirty dozen it’s misconception number 3: “A statistically significant finding is clinically important”.

2.  From [this paper](https://www.atsjournals.org/doi/abs/10.1164/rccm.202002-0281OC): “There was a statistically significant association between free cortisol and 90-day mortality (per 100nmol/L OR 1.13, 95%CI 1.00 to 1.27, p=0.04), although after a sensitivity analysis for missing covariates this association was no longer significant
    (OR 1.10, 95%CI 1.00 to 1.23, p=0.07).”

What’s wrong with this? On the plus side, they’ve given the odds ratios and confidence intervals, but they are implying a meaningful difference just because the p-value has moved across the magic 0.05 threshold.
The differences in the odds ratios and 95% confidence intervals are tiny and in my opinion the authors have poorly described their results.
In Steve Goodman’s dirty dozen it’s misconception number 4: “Studies with P values on opposite sides of 0.05 are conflicting”. This paper also had a lot of number 3’s.

So based on this tiny sample, combined with a wealth of other data from similar journals, I do not think that AJRCCM authors understand p-values.

## My pledge

Based on this latest experience and my exhaustion with dealing with p-values, I am making a pledge:

<center>
**There will be no p-values in any paper that I co-author in the next 12 months.**
</center>

If my co-authors insist on p-values, then I will take my name off the paper. I’ll try to get a statement in the acknowledgments like, “Adrian Barnett would have been an author, but it was him or the p-values.”

If journal editors or reviewers insist on p-values, then I will try to convince them otherwise and then either publish elsewhere or take my name off the paper.

Is this a gimmick? Possibly, but I’m really tired of people insisting on using a statistic that they don’t understand.
And “using” isn’t the right word, as the word I want would mean: “to abandon all other scientific thinking and any other available evidence”.
Perhaps “significancing”?

I’m hoping this one big decision will save me from a lot of little decisions.

Can I do it? A dozen months without a dirty dozen. Going cold Tukey (sic). I’ll report back in a year.

### Two minor caveats

1.  I reserve the right to use a Bayesian or bootstrap p-value.

2.  I can’t change papers in print.

### Reference

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-Goodman2008" class="csl-entry">

Goodman, Steven. 2008. “A Dirty Dozen: Twelve p-Value Misconceptions.” *Seminars in Hematology* 45 (3): 135–40. <https://doi.org/10.1053/j.seminhematol.2008.04.003>.

</div>

</div>
