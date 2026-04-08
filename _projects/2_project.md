---
layout: page
title: Model-Based Deep Learning for 3D Linear-Array PACT
description: Improving 3D photoacoustic imaging with multiview acquisition and deep learning reconstruction
img: assets/img/Multiview_DL_network.png
importance: 2
category: work
related_publications: true
---

## Project Overview

This project focuses on improving the three-dimensional imaging performance of linear-array photoacoustic computed tomography (PACT). It is based on our work currently under review in *IEEE Transactions on Biomedical Engineering (TBME)* {% cite miao_underreview_isotropic %}. Although linear-array systems are practical and widely used, they often suffer from limited elevational resolution, which reduces image quality and makes accurate volumetric visualization more difficult.

To address this limitation, I developed **MV-FISTA-Net**, a model-based deep learning framework that combines multiview acquisition with learnable iterative reconstruction. Built upon the multiview FISTA-based deconvolution framework, this method uses deep learning to recover finer structural details and improve volumetric image quality beyond what can be achieved with conventional iterative reconstruction alone.

I validated this framework using simulation, phantom, and in vivo human imaging datasets. Overall, this work demonstrates a computational strategy for improving the spatial resolution and reconstruction efficiency of 3D linear-array photoacoustic imaging.

## What I Did

In this project, I worked on the model design, training strategy, reconstruction framework, and experimental validation. This included developing the multiview deep learning architecture, designing the training pipeline, integrating model-based reconstruction with learnable components, and evaluating performance across synthetic and experimental datasets. The goal was to create a practical and scalable method for high-resolution 3D photoacoustic imaging.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Multiview_DL_network.png" title="MV-FISTA-Net architecture" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Multiview_DL_example.png" title="Representative imaging result" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: overview of the MV-FISTA-Net framework for multiview photoacoustic reconstruction. Right: representative imaging result showing improved vascular visualization with the proposed deep learning method.
</div>

## Why It Matters

A major challenge in linear-array photoacoustic tomography is that volumetric image quality is often limited by poor elevational resolution and the difficulty of recovering fine structural information from incomplete-view measurements. This project shows that combining multiview acquisition with model-based deep learning can improve both image sharpness and reconstruction quality, helping linear-array PACT move closer to high-resolution and computationally efficient 3D imaging.

## Outcome

This work demonstrates a practical strategy for improving the 3D imaging capability of linear-array photoacoustic systems through model-based deep learning. By combining multiview data acquisition with learnable reconstruction, the framework improves volumetric image fidelity and reconstruction speed while maintaining the flexibility and accessibility of linear-array imaging platforms.
