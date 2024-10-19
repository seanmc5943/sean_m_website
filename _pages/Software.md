---
layout: page
permalink: /software/
title: Software
description: Software packages in Stata or otherwise.
nav: true
nav_order: 3
---

#### [Inflate.ado](https://ideas.repec.org/c/boc/bocode/s459037.html)  
Inflate is a Stata program that inflates variables to real dollars using the U.S. Consumer Price Index (CPI). Useful for putting time series that vary across years, quarters, or months in real dollars, so you do not have to deal with merging in the CPI series yourself!

Note: The inflate command now requires an API key from FRED. This is because changes in FRED's data infrastructure forced the command to migrate from freduse to the built-in command import fred. A FRED API key may be obtained from [https://fred.stlouisfed.org/docs/api/api_key.html]

##### **Install**
Inflate is available on SSC. In Stata install by running:
\
&emsp; &emsp; ```ssc install inflate```

##### **Example**
###### The following code takes two monthly time series and puts them in real 2020 $.
Load in the nominal M1 and M2 money stocks from FRED.
\
&emsp; &emsp; ```freduse M1SL M2SL```
\
Make year and month variables.
\
&emsp; &emsp; ```gen year = year(daten)```
\
&emsp; &emsp; ```gen month = month(daten)```
\
Inflate both series to 2020 $.
\
&emsp; &emsp; ```inflate M1SL M2SL, year(year) month(month) end(2020)```
\
Now there are two new variables named M1SL_real and M2SL_real.
\
<img src="/assets/img/inflate_screen_grab-1400.webp" alt="Inflate Screenshot" width="70%"/>