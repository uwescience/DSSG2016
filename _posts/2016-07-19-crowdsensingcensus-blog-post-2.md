---
layout: post
title:  "OpenStreetMap: Mostly Amazing (Sometimes Troublesome)"
date:   2016-07-19
author: Rachael Dottle 
---


<p/> This past couple of weeks, part of the CrowdSensing Census team has been working on extracting, parsing and analyzing OpenStreetMap (OSM) data as a component of our heterogeneous-based tool for estimating poverty alongside call detail record (CDR) data. </p>

<p/>In our background research, we found previous [works](http:/arxiv.org/abs/1411.5204/) that investigated a means to estimate the spatial distribution of poverty with alternatives to census data. Such work uses OSM point of interest (POI) data and attempts to identify types of POIs (like fast food restaurants, pubs, etc.) that correlate with census variables and deprivation, in order to use such POI data to predict deprivation in a given neighborhood, city, or country. </p>

<p/> Based on these previous works, we set off analyzing OSM POI data and developed similar analyses that identify certain categorical POI that may correlate with our groundtruth census data for our test city, Milan. However, we immediately encountered a few issues when approaching OSM POI data. One major issue we faced was deciding which tool to use to extract large amounts of OSM data. </p>


<p/> There are many, many packages, libraries, APIs and user interfaces available to extract OSM data. However, not many of them are intuitive, nor do they provide us with exactly the kind of data we were looking for. Some packages allow us to extract large groups of OSM data in XML format, but may not include all the information we want (information like the timestamp of the map element or its complete list of tags). Other tools, like the osmar package in R, limit our extracts to a certain number of nodes and become buggy when we attempt to batch extract by a series of bounding areas. While we are able to extract a complete dataset using platforms like [BBBike Planet Extracts](http://extract.bbbike.org/), this method is not conducive to replicability. While we have extracted and begun analyzing OSM data for Milan, we continue to pine after a useful package or library that allows us to comprehensively call out complete OSM data, tags and all in a straightforward manner. </p>


<p/> Because OSM is an open-source mapping platform with crowd-sourced data, the data, once extracted, is rather unique. OSM POI can be identified by the tags users assign, but users do not always adhere to OSM conventions. In order to develop categories of POI that may be useful in our model, we first had to establish which tags to focus on. A common key tag assigned to POI in OSM is "[amenity](http:/wiki.openstreetmap.org/wiki/Key:amenity/)" (OSM tags have a key:value format, so a fast food restaurant might be tagged amenity=fast_food, for example). </p>

<p/> Once we filtered for only nodes tagged 'amenity', we found around 80 different value categories under the key 'amenity'. We then attempted to analyze the relationship between these distinct categories and our index of deprivation. </p>


<p/> Moving forward, we have a couple issues to address, and a million different ways we could continue to explore features available to us in OSM data. We are continuing to refine our method for extracting POI categories in order to account for mis-tagged nodes. We also hope to improve our method of differentiating between categories that might be relevant but have infrequent observations, like zoos, compared to categories that might not be relevant and have infrequent observations, like a mispelled 'amenity' key. 

Furthermore, OSM data has so much to offer beyond its POI nodes. Other works that have attempted to analyze the spatial distribution of deprivation took into account the urban fabric and built environment. OSM data includes dense street network data and building data. These data may provide us with alternative means to model spatial deprivation with OSM, which will improve our final model and analysis.  

Sidenote: The OSM State of the Map is this weekend, and the CrowdSensing Census team is very, very excited about it. ༼ つ ◕_◕ ༽つ

