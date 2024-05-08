---
layout: page
title: Detection of Fast Radio Bursts
description: My B.Sc. Final Year Project
img: /assets/img/projects/frb_detection/artists_impression.jpg
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" src="/assets/img/projects/frb_detection/artists_impression.jpg" title="Artist's impression of a Fast Radio Burst" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Artist's impression of a Fast Radio Burst. Image credit: CSIRO/Dr. Andrew Howells
</div>

Fast Radio Bursts (FRBs) are brief, bright flashes of radio waves that last only a few milliseconds of extragalactic origin. They are one of the most mysterious phenomena in astrophysics, and their progenitor(s) are still unknown.

The key characteristic of FRBs is their dispersion measure (DM) i.e. the frequency dependent delay due to electrons in the line of sight, and FRBs have DMs more than the Galactic contribution. DMs allow for study of FRBs' host galaxies, and combined with their polarization properties measured using rotation measure (RM), magnetars are thought to be the best candidate for FRB progenitors.

The first FRB was discovered while reviewing data in radio pulsar surveys taken using the Parkes Telescope {% cite Lorimer2007 %}. Since then, hundreds of FRBs have been discovered, especially using instruments with large FOVs such as the Canadian Hydrogen Intensity Mapping Experiment (CHIME).

I researched on developing and improving FRB detection codes, and wrote a standablone Python FRB detection program named the Python Language Radio Burst Emission Automatic Roger (PoLaR BEAR) based on a precursor program written in C++.
