---
title: "Dissertation Project"
date: 2019-08-15
tags: [Accident Analysis, Hotspots, Road Network Analysis]
header: 
  image: "/images/perceptron/AccidentAnalysis.jpg"
excerpt: "Traffic Accident Analysis, Accident Hotspots, EMS Response Time"
mathjax: "true"
---

# Spatial-Temporal Traffic Accident Analysis in relation to EMS Response Time

## Abstract
Traffic accidents constitute one of the dominant causes of death globally, influencing the welfare of modern society significantly. Aberdeen City is considered as one of the most traffic-congested cities in the UK, resulting in more than 180 incidents per year for the last 10-year period. The purpose of this study is to perform an accidents cluster analysis in the City of Aberdeen by examining both time and space aspects in relation to the Emergency Medical Services (EMS) response time. Performing network cluster analysis, new space-time accident hot spots are detected on the road network and then a composite examination between those hot spots and the EMS response time is performed.

Throughout the performed analysis and examination of the traffic accident data, some new accident trends have been identified, during the last few years. Moreover, a high density of accidents takes place during specific day hours and months. Finally, most of the hot spots are located within the boundaries of the HEAT standard of 8 minutes, constituting the EMS station ideally situated. However, an emphasis should be given on those hot spots located farther than the 8-minutes zones, and further policies should be deployed against those prone areas.

### Methodology
#### 1. Data Preparation
  Data cleansing and validation is achieved so that data to be ready for use by the GIS software. The datasets contain information about   traffic accidents in the UK, the road network and the location of the ambulance station. Afterwards, the data are analysed in a         spatial-temporal framework revealing interesting space-time patterns.
  * Study Area 
    <img src="{{ site.url }}{{ site.baseurl }}/images/perceptron/StudyArea.jpg" alt="linearly separable data">
  + Data Acquisition
    <img src="{{ site.url }}{{ site.baseurl }}/images/perceptron/DataAcq.jpg" alt="linearly separable data">

#### 2. Road Network Analysis
  The road network dataset which is acquired with a UK national coverage, contains information on virtually every road segment across     the UK. The road network was clipped into the extent of the boundaries of Aberdeen city in order to make the data manipulation           easier and faster.
  * EMS Response Time Distribution
    <img src="{{ site.url }}{{ site.baseurl }}/images/Dissertation/image.png" alt="linearly separable data">
      *The 'Find Closest Facility' tool was used to calculate the Distribution*
  + Space-time patterns and Emerging Hot spots
    <img src="{{ site.url }}{{ site.baseurl }}/images/Dissertation/EmergingHotSpot.jpg" alt="linearly separable data"><img src="{{           site.url }}{{ site.baseurl }}/images/Dissertation/SpaceTimeCube.jpg" alt="linearly separable data">
      *Used Tools*
      
    <img src="{{ site.url }}{{ site.baseurl }}/images/Dissertation/3D Visualization.jpg" alt="linearly separable data">
      *3D Visualization of the Space-Time Cubes*
   - Stopping Sight Distance (SSD)
      *The distance needed for a vehicle to stop before colliding with something in the roadway*
      $$SSD=(0.278*t*V)+V^2/(254*(f + G)$$
      
      where:
      
        $$SSD = Stopping\;Sight\;Distance$$
        $$t: Reaction\;Time\;in\;Seconds ≃ 1.5\;sec$$
        $$V: Car\;Speed\;in\;km/h ≃ road’s\;speed\;limit$$
        $$G: Slope\;level = 0$$               
        $$f: Coefficient\;of\;friction$$ <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Coefficient.JPG" alt="linearly separable data">

#### 3. Accident Analysis

### Results

  * Ambulance Service Areas and Find Closest Facilities Layers
    The Ambulance Service Areas Layer shows the regions that an ambulance can reach within different time-step intervals. In other           words, it refers to the time needed for an ambulance to reach the accident location and depends on the network complexity and the       road speed limit.<img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/ServiceAreas.jpg" alt="linearly separable data">
  * Space-time Hot Spot Analysis
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Clusters.jpg" alt="linearly separable data">
  * Accident Rates per Road
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/CpR.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/CaspR.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/DpR.jpg" alt="linearly separable data">
  * Accident hot spots comparison
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Cr_Cas.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Cr_D.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Cas_D.jpg" alt="linearly separable data">
  * Temporal Distributions
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Hourly.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Monthly.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Annual.jpg" alt="linearly separable data">
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Clock.JPG" alt="linearly separable data">
  * Accident Hot Spots and EMS Service Areas Comparison
    <img src="{{site.url }}{{ site.baseurl }}/images/Dissertation/Final.jpg" alt="linearly separable data">
    
<!---
### H3 Heading

Here's some basic text.

And here's some *italics*

Here's some **bold** text.

What about a [link](https://github.com/dataoptimal)?

Here's a bulleted list:
* First item
+ Second item
- Third item

Here's a numbered list:
1. First
2. Second
3. Third

Python code block:
```python
    import numpy as np

    def test_function(x, y):
      z = np.sum(x,y)
      return z
```

R code block:
```r
library(tidyverse)
df <- read_csv("some_file.csv")
head(df)
```

Here's some inline code `x+y`.

Here's an image:
<img src="{{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg" alt="linearly separable data">

Here's another image using Kramdown:
![alt]({{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg)

Here's some math:

$$z=x+y$$

You can also put it inline $$z=x+y$$
-->
