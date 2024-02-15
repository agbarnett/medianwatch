---
title: Here’s why you should (almost) never use a pie chart for your data
author: Adrian Barnett & Victor Oguoma
date: '2024-02-15'
draft: false
slug: pie_charts
tags:
  - statistics
subtitle: ''
description: ''
showtoc: no
image: '/img/path_4.jpg'
---

*Reproduced from [The Conversation](https://theconversation.com/heres-why-you-should-almost-never-use-a-pie-chart-for-your-data-214576)*

Our lives are becoming increasingly data driven. Our phones monitor our time and internet usage and online surveys discern our opinions and likes. These data harvests are used for telling us how well we’ve slept or what we might like to buy.

Numbers are becoming more important for everyday life, yet people’s numerical skills are falling behind. For example, the percentage of Year 12 schoolchildren in Australia taking higher and intermediate mathematics [has been declining for decades](https://amsi.org.au/?publications=year-12-participation-in-calculus-based-mathematics-subjects-takes-a-dive-2).

To help the average person understand big data and numbers, we often use visual summaries, such as pie charts. But while non-numerate folk will avoid numbers, most numerate folk will avoid pie charts. Here’s why.

# What is a pie chart?

A pie chart is a circular diagram that represents numerical percentages. The circle is divided into slices, with the size of each slice proportional to the category it represents. It is named because it resembles a sliced pie and can be “served” in many different ways.

An example pie chart below shows Australia’s two-party preferred vote before the last election, with Labor on 55% and the the Coalition on 45%. The two near semi-circles show the relatively tight race – this is a useful example of a pie chart.

![](/img/pie_polls2.jpg){width=650px} 

# What’s wrong with pie charts?

Once we have more than two categories, pie charts can easily misrepresent percentages and become hard to read.

The three charts below are a good example – it is very hard to work out which of the five areas is the largest. The pie chart’s circularity means the areas lack a common reference point.

![](/img/1280px-Piecharts_half.png){width=650px} 

Pie charts also do badly when there are lots of categories. For example, this chart from a study on data sources used for COVID data visualisation shows hundreds of categories in one pie.

![](/img/informatics-07-00035-g005.png){width=650px} 

The tiny slices, lack of clear labelling and the kaleidoscope of colours make interpretation difficult for anyone.

It’s even harder for a colour blind person. For example, this is a simulation of what the above chart would look like to a person with deuteranomaly or reduced sensitivity to green light. This is the most common type of colour blindness, affecting roughly [4.6% of the population](https://wearecolorblind.com/articles/a-quick-introduction-to-color-blindness/).

It can get even worse if we take pie charts and make them three-dimensional. This can lead to egregious misrepresentations of data.

Below, the yellow, red and green areas are all the same size (one-third), but appear to be different based on the angle and which slice is placed at the bottom of the pie.

![](/img/three_areas.png){width=650px} 

# So why are pie charts everywhere?

Despite the well known problems with pie charts, they are everywhere. They are in journal articles, PhD theses, political polling, books, newspapers and government reports. They’ve even been used by the Australian Bureau of Statistics.

While statisticians have criticised them for decades, it’s hard to argue with this logic: “if pie charts are so bad, why are there so many of them?”

Possibly they are popular because they are popular, which is a circular argument that suits a pie chart.

![](/img/collage.png){width=650px} 
# What’s a good alternative to pie charts?

There’s a simple fix that can effectively summarise big data in a small space and still allow creative colour schemes.


It’s the humble bar chart. Remember the brain-aching pie chart example above with the five categories? Here’s the same example using bars – we can now instantly see which category is the largest.


![](/img/1280px-Piecharts.png){width=650px} 

Linear bars are easier on the eye than the non-linear segments of a pie chart. But beware the temptation to make a humble bar chart look more interesting by adding a 3D effect. As you already saw, 3D charts distort perception and make it harder to find a reference point.

Below is a standard bar chart and a 3D alternative of the number of voters in the 1992 US presidential election split by family income (from under US$15K to over $75k). Using the 3D version, can you tell the number of voters for each candidate in the highest income category? Not easily.

![](/img/3d_bars.png){width=650px} 

# Is it ever okay to use a pie chart?

We’ve shown some of the worst examples of pie charts to make a point. Pie charts can be okay when there are just a few categories and the percentages are dissimilar, for example with one large and one small category.

Overall, it is best to use pie charts sparingly, especially when there is a more “digestible” alternative – the bar chart.

Whenever we see pie charts, we think one of two things: their creators don’t know what they’re doing, or they know what they are doing and are deliberately trying to mislead.

A graphical summary aims to easily and quickly communicate the data. If you feel the need to spruce it up, you’re likely reducing understanding without meaning to do so.




