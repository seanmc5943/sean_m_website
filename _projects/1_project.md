---
layout: page
title: Saiz Maps
description: Visualization of Saiz's Geographic Determinants of Housing Supply"
img: assets/img/new_york.png
importance: 1
category: work
---

An important paper in the housing supply literature is "The Geographic Determinants of Housing Supply" by Albert Saiz, which estimates the amount of area within 50km of major U.S. city centers that is undevelopable due to geographic features like ocean, wetlands, and mountainous terrain. For the purposes of the paper, land is considered undevelopable either because it is covered with water or has a slope of greater than 15 percent. He concludes that geography plays a large role in urban growth not only by directly reducing land availability, but also by increasing land values and incentivizing regulatory constraints on land use. 

However, at least in the final published form of the paper, there are no maps of these cities. Below are maps of two major American cities I made from satellite data where white space is geographic area that is difficult or impossible to build on. Each map is the area within 30 miles of a city center and purple denotes census tracts with higher density of <a href="https://github.com/microsoft/USBuildingFootprints"> building footprints</a>.  Many will recognize that the left image is San Francisco, CA—but what about the city in the right image?

<table><tr>
        <td> <img src="assets/img/san_francisco.png" alt="san_francisco" width="325"/>  </td>
        <td> <img src="assets/img/atlanta.png" alt="atlanta" width="325"/> </td>
    <tr/></table>
    
<img src="assets/img/colorscale_tracts.png" alt="colorscale_tracts" width="275"/> 

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
