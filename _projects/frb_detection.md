---
layout: page
title: Detection of Fast Radio Bursts
description: My B.Sc. Final Year Project
img: /assets/img/projects/frb_detection/artists_impression.jpg
importance: 9
related_publications: true
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="/assets/img/projects/frb_detection/artists_impression.jpg" title="Artist's impression of a Fast Radio Burst" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Artist's impression of a Fast Radio Burst. Image credit: CSIRO/Dr. Andrew Howells
</div>

Fast Radio Bursts (FRBs) are brief, bright flashes of radio waves that last only a few milliseconds of extragalactic origin. They are one of the most mysterious phenomena in astrophysics, and their progenitor(s) are still unknown.

The key characteristic of FRBs is their dispersion measure (DM) i.e. the frequency dependent delay due to electrons in the line of sight, and FRBs have DMs more than the Galactic contribution. DMs allow for study of FRBs' host galaxies, and combined with their polarization properties measured using rotation measure (RM), magnetars are thought to be the best candidate for FRB progenitors.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="/assets/img/projects/frb_detection/lorimer.jpg" title="Lorimer Burst" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Waterfall plot of the first FRB discovered, FRB 010724.
</div>

The first FRB was discovered while reviewing data in radio pulsar surveys taken using the Parkes Telescope {% cite Lorimer2007 --file references %}. Since then, hundreds of FRBs have been discovered, especially using instruments with large FOVs such as the Five-hundred-meter Aperture Spherical Telescope (FAST) and the Canadian Hydrogen Intensity Mapping Experiment (CHIME).

Previously, FRB detection are performed using pulsar signal processing programs (e.g. SIGPROC and PRESTO). Currently, there are various FRB detection codes available, mainly optimizing the computationally intensive dedispersion process. One of them is the Burst Emission Automatic Roger (BEAR) program, which is a standalone C++ pipeline for FRB detection developed for various Chinese telescopes {% cite Men2019 --file references %}.

I researched on developing and improving FRB detection codes, and wrote a standablone Python FRB detection program named the Python Language Radio Burst Emission Automatic Roger (PoLaR BEAR) based on BEAR. A repository of the script and my thesis is avaiable on [GitHub](https://github.com/affanadly/PoLaR-BEAR).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="/assets/img/projects/frb_detection/polar_bear.jpeg" title="PoLaR BEAR Output" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example output of PoLaR BEAR for FRB121102
</div>
