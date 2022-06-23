---
layout: page
title: San Francisco House Prices
description: Interactive map of San Francisco housing prices back to the 1970s.
img: assets/img/sf-sj-3d-resize.png
importance: 2
category: mapping
---

Here is a tract-level interactive map where mean house value is represented by the tract's height in San Francisco and San Jose housing markets starting from the 1970 Decennial Census through the 2014-2018 American Community Survey (ACS).  Clicking on a tract displays the mean house value and mean contract rent in the selected Decennial Census year. Look up your address to see what a typical house in your neighborhood would cost in the 1970s. <a href='https://seanmc5943.github.io/sfsj_3d.html'>Full Screen</a>
<iframe src="https://seanmc5943.github.io/sfsj_3d.html"  style='display: block;' width='100%' height='600px' scrolling='no'></iframe>
<br>

### Notes on Data
All data from the US censuses and the ACS were retrieved from the <a href='https://www.nhgis.org/'>NHGIS</a>.

The geographic boundaries of census tracts may change across censuses. To better harmonize the data across time, I use the areal interpolation weights provided by the <a href='https://s4.ad.brown.edu/projects/diversity/Researcher/Bridging.htm'>Longitudinal Tract Database</a>, which update the old tract geometries to 2010 census tract boundaries.

Mean house values are inflated to real 2020 dollars based on the first half average of 2020 and the average annual <a href='https://data.bls.gov/cgi-bin/surveymost?cu'>CPIs</a> for more consistent comparison across time.  The extruded height of each census tract is (inflated mean house value / 100) meters off the map. Individual tract mean house values may suffer from measurement error for a few reasons:
1. For tracts where aggregate value is not reported, mean values are calculated based on a weighted sum of the counts for each house value bracket e.g. the number of houses that cost \$300,000 to \$400,000 times \$350,000. For the top value bracket, e.g. $1,000,000 or more, I assume 1.5*top value.
2. Converting the old tract geometries to the current 2010 geometries is far from perfect. Scaling and combining the counts based on geographic areal interpolation introduces potential measurement error.

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
