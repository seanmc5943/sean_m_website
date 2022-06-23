---
layout: page
title: Saiz Maps
description: Visualization of Saiz's Geographic Determinants of Housing Supply
img: /assets/img/new_york.png
importance: 1
category: mapping
---

An important paper in the housing supply literature is "The Geographic Determinants of Housing Supply" by Albert Saiz, which estimates the amount of area within 50km of major U.S. city centers that is undevelopable due to geographic features like ocean, wetlands, and mountainous terrain. For the purposes of the paper, land is considered undevelopable either because it is covered with water or has a slope of greater than 15 percent. He concludes that geography plays a large role in urban growth not only by directly reducing land availability, but also by increasing land values and incentivizing regulatory constraints on land use. 

However, at least in the final published form of the paper, there are no maps of these cities. Below are maps of two major American cities I made from satellite data where white space is geographic area that is difficult or impossible to build on. Each map is the area within 30 miles of a city center and purple denotes census tracts with higher density of <a href="https://github.com/microsoft/USBuildingFootprints"> building footprints</a>.  Many will recognize that the left image is San Francisco, CA—but what about the city in the right image?


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/san_francisco.png" title="San Francisco" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="/assets/img/atlanta.png" title="Atlanta" class="img-fluid" %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0"></div>
    <div class="col-sm mt-3 mt-md-0">
         {% include figure.html path="/assets/img/colorscale_tracts.png" title="Color Scale" class="img-fluid" %}        
    </div>
    <div class="col-sm mt-3 mt-md-0"></div>

</div>

The map on the right is Atlanta, GA. It is clear that there is much less land available for development in San Francisco and these maps, even by themselves, strongly suggest that the lack of available land factors heavily into the high house prices in San Francisco today (see Saiz for a deeper discussion).
Below are high resolution maps for the twelve largest U.S. metropolitan areas (ordered by population):

<div class="caption">New York City</div>
{% include figure.html path="/assets/img/new_york.png" title="new_york" class="img-fluid" %} 

<div class="caption">Los Angeles</div>
{% include figure.html path="/assets/img/los_angeles.png" title="los_angeles" class="img-fluid" %} 

<div class="caption">Chicago</div>
{% include figure.html path="/assets/img/chicago.png" title="chicago" class="img-fluid" %} 

<div class="caption">Dallas</div>
{% include figure.html path="/assets/img/dallas.png" title="dallas" class="img-fluid" %} 

<div class="caption">Houston</div>
{% include figure.html path="/assets/img/houston.png" title="houston" class="img-fluid" %} 

<div class="caption">Washington D.C.</div>
{% include figure.html path="/assets/img/washington_DC.png" title="washington_DC" class="img-fluid" %} 

<div class="caption">Miami</div>
{% include figure.html path="/assets/img/miami.png" title="miami" class="img-fluid" %} 

<div class="caption">Philadelphia</div>
{% include figure.html path="/assets/img/philadelphia.png" title="philadelphia" class="img-fluid" %} 

<div class="caption">Atlanta</div>
{% include figure.html path="/assets/img/atlanta.png" title="atlanta" class="img-fluid" %} 

<div class="caption">Boston</div>
{% include figure.html path="/assets/img/boston.png" title="boston" class="img-fluid" %} 

<div class="caption">Phoenix</div>
{% include figure.html path="/assets/img/phoenix.png" title="phoenix" class="img-fluid" %} 

<div class="caption">San Francisco</div>
{% include figure.html path="/assets/img/san_francisco.png" title="san_francisco" class="img-fluid" %} 

#### References & Mapbox Attribution
Saiz, Albert. *The Geographic Determinants of Housing Supply*. Quarterly Journal of Economics 125, 3 (2010) 

Elevation data retrieved from the <a href='https://viewer.nationalmap.gov/basic/'>United States Geological Survey</a> \
Water data retrieved from <a href='https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html'>U.S. Census TIGER/Line Shapefiles</a> 

© <a href='https://www.mapbox.com/about/maps/'>Mapbox</a> © <a href='http://www.openstreetmap.org/copyright'>OpenStreetMap</a> <strong>
