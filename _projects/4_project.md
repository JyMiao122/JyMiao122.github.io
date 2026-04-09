---
layout: page
title: Transducer and Optics Design for Linear-Array Spine Imaging
description: Integrated linear-array transducer, fiber, and optics design for future clinical photoacoustic spine imaging
img: assets/img/spine_design.png
importance: 5
category: work
related_publications: false
---

## Project Overview

This project focuses on the integrated design of a linear-array transducer, optical illumination module, and mechanical package for future clinical photoacoustic spine imaging. The goal is to develop a compact and clinically practical probe architecture that combines efficient light delivery, acoustic detection, and mechanically constrained packaging in a single platform.

A central design requirement of this work is to achieve effective optical illumination while maintaining compatibility with a required transducer focal depth of 10 mm. To address this, I designed a 3D fiber–optics–transducer package in which the optical and acoustic subsystems were co-optimized rather than treated independently. The design considered illumination efficiency, light overlap, probe footprint, bottom contact area, and manufacturable packaging geometry for eventual translational use.

Overall, this project establishes an engineering framework for integrating optics and ultrasound hardware into a compact linear-array photoacoustic probe suitable for future spine-related clinical applications.

## What I Did

In this project, I designed the optical and acoustic architecture of the probe, including the geometric arrangement of the linear-array transducer, optical fibers, prism-based illumination path, and outer package. I used **Zemax** to simulate optical beam propagation and evaluate how fiber position, prism geometry, and package dimensions affect light steering and overlap in the target imaging region.

I also analyzed packaging trade-offs between total probe size and usable bottom contact area, with the goal of maintaining efficient and well-controlled illumination in a compact form factor. This included refining the optical path to avoid undesirable beam behavior such as premature convergence inside the prism or direct light leakage from the bottom surface.

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/spine_design.png" title="Overall transducer and optics package design" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overall 3D design of the integrated fiber, optics, and linear-array transducer package for future clinical photoacoustic spine imaging.
</div>

## Design Features

The probe concept integrates fused-input optical fibers with a prism-based illumination module and a linear-array transducer to support efficient photoacoustic excitation and signal detection within a compact housing. The use of fused-input fibers was selected to improve optical throughput and reduce loss, supporting high-energy delivery for photoacoustic imaging.

The optical design was developed to achieve controlled beam overlap within the desired imaging region while satisfying geometric packaging constraints. Fiber placement relative to the prism was tuned to shape the overlap region, and the prism dimensions were evaluated to avoid unfavorable beam behavior such as excessive internal convergence or unintended light escape from the bottom surface. These considerations were balanced against the limited bottom contact area required for practical probe interfacing.

In parallel, the transducer and optical subsystems were designed around a required acoustic focus of 10 mm so that the optical illumination region and acoustic sensitivity region could be better aligned for future imaging performance.

## Why It Matters

Photoacoustic spine imaging presents a challenging design problem because the probe must simultaneously provide efficient optical illumination, appropriate acoustic focusing, and a physically compact form factor. Unlike benchtop optical layouts, a clinically relevant probe must operate under tight spatial constraints while preserving illumination quality and acoustic sensitivity.

This project addresses that challenge through integrated co-design of the optics, transducer geometry, and mechanical package. By treating illumination delivery, acoustic focus, and packaging constraints as a unified design problem, this work moves toward a more practical probe architecture for translational linear-array photoacoustic imaging.

## Outcome

This project established a compact transducer–fiber–optics design framework for future clinical photoacoustic spine imaging. The work defined key geometric and optical trade-offs related to focal depth, beam overlap, prism size, and package dimensions, and used Zemax simulation to guide optical design decisions within a clinically constrained form factor. Overall, it provides a foundation for future prototype fabrication, experimental validation, and eventual translation of linear-array photoacoustic imaging toward spine applications.
