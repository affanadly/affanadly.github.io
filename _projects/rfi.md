---
layout: page
title: RFI Mitigation using Spectral Kurtosis
img: /assets/img/projects/rfi/starlink.jpg
importance: 1
related_publications: true
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="/assets/img/projects/rfi/starlink.jpg" title="Starlink" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Starlink satellite interfering an image of the double star Albireo. Image credit: Rafael Schmall
</div>

Radio frequency interference poses a significant challenge in radio astronomy, often leading to data inaccuracies and rendering observations unusable especially in the modern era of wireless devices and telecommunication. Effective RFI monitoring is essential in the site selection process before constructing radio astronomy observatories, followed by mitigation strategies to minimize its adverse effects.

We modify the spectral kurtosis (SK) algorithm which utilizes high-order statistics to flag for RFI {% cite Nita2010 --file references %}, with the main goal of reducing the influence of highly-contaminated channels. Using data from RFI monitoring in urban and rural areas in Malaysia, we are able to verify the suitability of rural areas for radio astronomy observations. RFI patterns detected using the algorithm match spectrum allocations, along with the presence of few physical phenomena.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="/assets/img/projects/rfi/map.png" title="Map of RFI Monitoring" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Map of RFI monitoring sites in Malaysia.
</div>

I was involved in the data analysis and interpretation, as well as the writing of the manuscript.
