---
layout: post
author: Kara Woo
date:   2016-07-15
title: Unsafe Foods Team Visits the Department of Health
---


The [Unsafe Foods](http://escience.washington.edu/dssg/project-summaries-2016/)
team began week 4 with a field trip to the Washington State Department of
Health's Division of Disease Control & Health Statistics. We met with state
epidemiologists who gave us insight into their process for monitoring foodborne
illness outbreaks and recommending that food products be recalled. 

Determining the source of a foodborne illness outbreak is a difficult process,
in part because most people who get food poisoning do not seek medical care. In
cases when a person does visit a doctor, the doctor may or may not order testing
to diagnose the patient. If the testing reveals certain pathogens, such as
_Salmonella_, the laboratory must notify the local health jurisdiction, which
then conducts interviews with the patient to find out everything they have
eaten. The local health jurisdiction also takes the samples of the pathogen from
the lab and analyzes them to see if the strain matches other patients who have
previously become sick. This process may be repeated many times for many
patients before the source of the outbreak is clear and a recall can proceed.

<figure>
  <img 
  src="{{ site.url }}/assets/images/cdc-salmonella.jpg"
  alt="Outbreak and recall of Salmonella from imported cucumbers">
  <figcaption style="font-size:12px">
    Outbreak and recall of <i>Salmonella</i> Poona from imported cucumbers.
    Source: 
    <a href="http://www.cdc.gov/salmonella/poona-09-15/epi.html">CDC</a>.
  </figcaption>
</figure>

<br>

Hearing from the Department of Health helped us better understand the recall
process and put our project in context. We presented our project to them as
well, and we had a fruitful discussion about some possible next steps.

This week we have also made great progress combining our disparate data sources
into a PostgreSQL database. Thanks to
[Cynthia's]({{ site.url }}/2016/06/24/cynthia-intro.html) 
database expertise, we are well on our way to having a unified database we can
use to make connections between online product reviews and product recalls.

<figure>
  <img
  src="{{ site.url }}/assets/images/unsafe-foods-db.png"
  alt="Database schema">
  <figcaption style="font-size:12px">
    Database schema
  </figcaption>
</figure>
