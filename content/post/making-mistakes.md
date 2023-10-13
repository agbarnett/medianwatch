---
title: "Mistakes, I’ve made a few, but then again, not too few to mention"
author: "Adrian Barnett"
date: 2020-03-17
categories: []
tags: ["statistics","mistakes"]
slug: making-mistakes
showtoc: false
image: "/img/rail_1.jpg"
bibliography: bibliography.bib
link-citations: true
---

### Statistics can be hard

Here’s a great quote about working with statistics from the fantastic statistician [David Spiegelhalter](http://www.statslab.cam.ac.uk/~david/): “I am often asked why people tend to find probability a difficult and unintuitive idea, and I reply that, after forty years researching and teaching in this area, I have finally concluded that it is because probability really *is* a difficult and unintuitive idea” ([Spiegelhalter 2019](#ref-Spiegelhalter2019)).

Someone who attended my one-day statistics refresher course expressed disappointment in their evaluation that after a day’s training they did not now feel like an expert. Perhaps if I’d given a course in *Microsoft Paint* I could have handed out certificates that rightly said “certified expert”, but statistics is not something you can master in a day.

### Mistakes

One consequence of statistics being hard is that mistakes are made. Far too often researchers use the wrong statistical methods, or use shoddy data, or misinterpret the statistics.

And I’ve made mistakes too. Just last week I noticed a mistake in my R code that substantively changed the results of a survey analysis. Luckily I spotted this before we sent the paper for review, but it was a near miss.

I made a big mistake in one of my first ever publications by using the wrong intra-cluster correlation ([Underwood, Barnett, and Hajioff 1998](#ref-Underwood1988)), which was kindly corrected by Sally Kerry and Martin Bland (more from him below) ([Kerry and Bland 1998](#ref-Kerry1998)).

I made a mistake in my most highly cited paper ([Barnett, Pols, and Dobson 2004](#ref-Barnett2004)). I found this one years later when I was moving the code from an old web site to *GitHub* ([Barnett, Van Der Pols, and Dobson 2015](#ref-Barnett2015IJE)). The calculations were right on the web site, but wrong in the paper. I have no idea how this happened, possibly just a transcription error as I was fiddling with the parameters in the example between the web and the paper. This is a regrettable mistake because this paper has been widely cited and read.

I made a mistake in one of my most influential papers on the time that Australian researchers spend applying for funding ([Herbert et al. 2013](#ref-Herbert2013)). Here I accidentally used the number of chief investigators rather than the distribution of chief investigators. This means the total time that researchers spend applying for funding should be 604 years not 551. A fairly big difference that does cause me chagrin. My comfort is that I think the impact of the paper would have been the same with either figure, as both are shocking.

I even made a minor mistake in my first [blog article](https://medianwatch.netlify.com/post/funding-gender-disparity), as I didn’t label what the error bars were (fixed now).

There are likely other mistakes that I’ve missed and have been published because neither my colleagues or the peer reviewers spotted them. With bigger data sets with huge numbers of rows and columns, mistakes are now more likely. I think a big part of the current reproducibility crisis is caused by errors in statistical analyses.

### Martin Bland

Back in 2002 when I was an early career researcher, I saw the great statistician Martin Bland give an hour-long talk about his own statistical mistakes. This remains one of the most memorable talks I have ever attended. I found it incredibly empowering to realise that someone so talented still made mistakes. I felt like Martin had given me a licence to fail, but that also gave me a licence to try.

This might sound like I’m encouraging slap-dash practices, as if statistics were karaoke where you get praised for having the nerve to do it rather than what you sound like. In reality there are real consequences for getting statistics wrong. To keep this blog topical, I’ve seen multiple legitimate warnings on *Twitter* just this week about people “having a go” with data on COVID-19.

I am still advocating for lots of background reading, lots of training (in theory and practice), and lots of data and code checking. But I’m also saying that you are likely to make mistakes given that we work in such a complex area.

Another benefit to making mistakes is that I am good at spotting mistakes when I review papers, because I’ve remembered the tell-tale signs of my past mistakes.
A key part of Martin’s talk was about learning from his mistakes and then avoiding them.

### The final curtain

I’m now going to brazenly compare myself to Martin and hope that my admissions of mistakes will similarly empower other statisticians. I also hope that these admissions do not destroy my career; Martin has survived pretty well!

For what else could I do? I’ve travelled each and every statistical by way (one-way and two-way), and more, much more than this, I analysed it my way.

#### References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-Barnett2004" class="csl-entry">

Barnett, Adrian G, Jolieke C van der Pols, and Annette J Dobson. 2004. “Regression to the Mean: What It Is and How to Deal with It.” *International Journal of Epidemiology* 34 (1): 215–20. <https://doi.org/10.1093/ije/dyh299>.

</div>

<div id="ref-Barnett2015IJE" class="csl-entry">

Barnett, Adrian G, Jolieke C Van Der Pols, and Annette J Dobson. 2015. “Correction to: Regression to the Mean: What It Is and How to Deal with It.” *International Journal of Epidemiology* 44 (5): 1748–48. <https://doi.org/10.1093/ije/dyv161>.

</div>

<div id="ref-Herbert2013" class="csl-entry">

Herbert, Danielle L, Adrian G Barnett, Philip Clarke, and Nicholas Graves. 2013. “On the Time Spent Preparing Grant Proposals: An Observational Study of Australian Researchers.” *BMJ Open* 3 (5). <https://doi.org/10.1136/bmjopen-2013-002800>.

</div>

<div id="ref-Kerry1998" class="csl-entry">

Kerry, S, and M Bland. 1998. “Cluster Randomization.” *British Journal of General Practice* 48 (431): 1342.

</div>

<div id="ref-Spiegelhalter2019" class="csl-entry">

Spiegelhalter, D. 2019. *The Art of Statistics: How to Learn from Data*. Basic Books. <https://books.google.com.au/books?id=4qWFDwAAQBAJ>.

</div>

<div id="ref-Underwood1988" class="csl-entry">

Underwood, M, A Barnett, and S Hajioff. 1998. “Cluster Randomization: A Trap for the Unwary.” *British Journal of General Practice* 48 (428): 1089–90. <https://bjgp.org/content/48/428/1089>.

</div>

</div>
