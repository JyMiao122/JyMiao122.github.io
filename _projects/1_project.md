---
layout: page
title: Multiview Linear-Array PACT
description: Improving 3D photoacoustic imaging with multiview acquisition and reconstruction
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

## Project Overview

This project focuses on improving the three-dimensional imaging performance of linear-array photoacoustic computed tomography (PACT). Linear-array systems are widely used because they are compact, practical, and compatible with handheld imaging, but they often suffer from poor resolution in the elevational direction. This anisotropic resolution limits the quality of 3D visualization and makes it difficult to accurately recover fine structures.

To address this challenge, I developed a **multiview linear-array PACT (MvLPACT)** framework that combines data acquired from multiple viewing angles and reconstructs the final volume using a **multiview FISTA-based deconvolution method**. By integrating complementary information from different views, this approach improves volumetric image quality and substantially enhances elevational resolution compared with conventional single-view imaging.

I validated this framework through both phantom studies and in vivo human imaging experiments. Overall, this work provides a practical way to extend the capabilities of linear-array photoacoustic systems while preserving their accessibility and flexibility.

## My Contribution

In this project, I worked on the development of the multiview imaging framework, reconstruction strategy, experimental design, and validation. This included building the multiview acquisition pipeline, implementing the reconstruction algorithm, and evaluating performance through quantitative and experimental comparisons. The goal was to create a practical method for achieving higher-quality 3D photoacoustic imaging without relying on more complex or less accessible imaging geometries.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project1_1.jpg" title="MvLPACT system overview" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project1_2.jpg" title="Multiview scanning setup" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project1_3.jpg" title="In vivo imaging demonstration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Representative views of the multiview linear-array photoacoustic imaging system, acquisition setup, and experimental demonstration.
</div>

## Why It Matters

A major challenge in linear-array photoacoustic tomography is that image resolution is not uniform in all three dimensions. In particular, the relatively poor elevational resolution can blur structures and reduce the accuracy of 3D visualization. This project shows that multiview acquisition, combined with physics-guided reconstruction, can help overcome this limitation and move linear-array PACT closer to robust high-quality volumetric imaging for biomedical applications.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project1_4.jpg" title="Resolution improvement results" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project1_5.jpg" title="3D reconstruction example" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example reconstruction results and quantitative comparisons showing improved elevational resolution with the proposed multiview framework.
</div>

## Outcome

This work demonstrates a practical strategy for improving the 3D imaging capability of linear-array photoacoustic systems. By combining multiview acquisition with model-based reconstruction, the framework improves volumetric image fidelity while maintaining the simplicity and usability of linear-array imaging platforms.
