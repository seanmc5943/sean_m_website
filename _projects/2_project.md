---
layout: page
title: San Francisco House Prices
description: Interactive map of San Francisco housing prices back to the 1970s.
img: /assets/img/sf-sj-3d-resize.png
importance: 2
category: mapping
---

I present a tract-level interactive map of San Francisco's mean house values in constant 2020 $ starting from the 1970 Decennial Census all the way through the 2014-2018 American Community Survey (ACS). Each tract's height and color signifies its mean house value.  The tracts' heights paint a stark picture of the absolute growth in real house prices and reveal significant heterogeneity across different neighborhoods in the Bay Area.  Clicking a tract displays the mean house value and mean contract rent in the selected Decennial Census year. <a href='https://seanmc5943.github.io/sfsj_3d.html'>Full Screen</a>
<iframe src="https://seanmc5943.github.io/sfsj_3d.html"  style='display: block;' width='100%' height='600px' scrolling='no'></iframe>
<br>

### Notes on Data
All data from the US censuses and the ACS were retrieved from the <a href='https://www.nhgis.org/'>NHGIS</a>.

The geographic boundaries of census tracts may change across censuses. To better harmonize the data across time, I use the areal interpolation weights provided by the <a href='https://s4.ad.brown.edu/projects/diversity/Researcher/Bridging.htm'>Longitudinal Tract Database</a>, which update the old tract geometries to 2010 census tract boundaries.

Mean house values are inflated to real 2020 dollars based on the first half average of 2020 and the average annual <a href='https://data.bls.gov/cgi-bin/surveymost?cu'>CPIs</a> for more consistent comparison across time.  The extruded height of each census tract is (inflated mean house value / 100) meters off the map. Individual tract mean house values may suffer from measurement error for a few reasons:
1. For tracts where aggregate value is not reported, mean values are calculated based on a weighted sum of the counts for each house value bracket e.g. the number of houses that cost \$300,000 to \$400,000 times \$350,000. For the top value bracket, e.g. $1,000,000 or more, I assume 1.5*top value.
2. Converting the old tract geometries to the current 2010 geometries is far from perfect. Scaling and combining the counts based on geographic areal interpolation introduces potential measurement error.