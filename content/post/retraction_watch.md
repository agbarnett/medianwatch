---
title: Checking BibTeX files against the Retraction Watch database
author: Adrian Barnett
date: '2024-03-12'
draft: false
slug: retraction_watch
tags:
  - retractions
  - integrity
subtitle: ''
description: ''
showtoc: no
image: '/img/alley_1.jpg'
---

Last week I saw [Alison Avenell](https://www.abdn.ac.uk/people/a.avenell) give a great talk titled "Improving the integrity of published research: How, when, and if?’’ This was on her experience of finding fraudulent papers and what actions the journals took to correct the record -- which was too often nothing. 

One of Alison's recommendations was to avoid inadvertently citing retracted papers by checking against the wonderful [*Retraction Watch*](https://retractionwatch.com/) database. For those using reference management software such as *Zotero* this is already done for you.

I write most papers in *LaTeX* or *Overleaf* which means my references are in *BibTeX* and hence do not get checked against *Retraction Watch*. So I have written an app (available [here](https://aushsi.shinyapps.io/retraction_watch_bib/)) that extracts the DOIs from a *BibTeX* file and checks them against the latest *Retraction Watch* database.

*Retraction Watch* are a vital resource in research integrity and their "Weekend reads" are a must read. I am also grateful that [*Crossref*](https://www.crossref.org/) make accessing the database super easy.
