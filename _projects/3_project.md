---
layout: page
title: PAUSIV for Breast Biopsy Clip Localization
description: Real-time photoacoustic and ultrasound imaging for biopsy clip detection in breast surgery
img: assets/img/Clip_f1.png
importance: 3
category: work
related_publications: false
---

## Project Overview

This project focuses on developing **PAUSIV**, a photoacoustic/ultrasound imaging platform for real-time localization of biopsy marker clips in breast cancer surgery. In breast-conserving procedures, accurate localization of non-palpable lesions remains a major challenge, and current approaches often require additional preoperative localization procedures such as wires, seeds, or tags. PAUSIV was designed to provide a wire-free, radiation-free, and workflow-compatible alternative by directly visualizing biopsy clips with high contrast during imaging.

A central motivation of this work is to improve surgical guidance while reducing patient burden and procedural complexity. Because titanium biopsy clips generate strong photoacoustic contrast relative to surrounding tissue, they can serve as effective imaging targets for localization. By combining photoacoustic imaging with co-registered ultrasound, PAUSIV enables both structural guidance and clip-specific visualization within the same platform.

I validated this system through both ex vivo breast specimen studies and in vivo human imaging. Overall, this work demonstrates the feasibility of using photoacoustic/ultrasound imaging for accurate and clinically practical biopsy clip localization in breast cancer care.

## What I Did

In this project, I worked on the imaging platform development, experimental design, image reconstruction, and deep-learning-based detection framework. This included optimizing the photoacoustic/ultrasound imaging system for clip visualization, designing and conducting ex vivo and in vivo validation studies, and developing a real-time clip localization model that incorporated both imaging features and clinical prior information. The goal was to create a practical platform for reliable biopsy clip detection during breast imaging and surgical guidance.

<div class="row">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Clip_f1.png" title="Ex vivo biopsy clip visualization" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Representative ex vivo breast specimen with corresponding biopsy clip localization result.
</div>

<div class="row">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Clip_f2.png" title="Clip detection pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the deep-learning-based pipeline for biopsy clip detection in photoacoustic images.
</div>

The system was first evaluated on ex vivo breast tissue specimens obtained in the operating room, where X-ray imaging served as the ground truth for clip location before photoacoustic imaging and reconstruction. PAUSIV demonstrated strong clip conspicuity, with clip signals substantially exceeding background tissue signals and providing markedly higher contrast than ultrasound alone. To support translation into clinical use, the imaging framework was further extended with a deep-learning-based clip detection model trained using ex vivo and in vivo data.

<div class="row">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Clip_f3.png" title="In vivo PAUSIV validation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Representative in vivo breast imaging results showing PA, US, and PA/US overlay images for biopsy clip localization.
</div>

<div class="row">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Clip_f4.png" title="Real-time in vivo clip detection" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Real-time in vivo clip detection results showing stable localization across consecutive photoacoustic frames.
</div>

## Why It Matters

A major challenge in breast-conserving surgery is the accurate localization of biopsy markers associated with non-palpable lesions. Existing localization approaches often require separate preoperative procedures, can increase patient burden, and may complicate surgical workflow. This project shows that photoacoustic/ultrasound imaging can provide direct, real-time visualization of biopsy clips with strong contrast, offering a promising alternative that is both wire-free and compatible with clinical practice.

In addition, the integration of deep learning improves robustness under realistic clinical variability, including differences in tissue composition, clip depth, and patient anatomy. This makes the system more suitable for practical real-time guidance and broadens its potential clinical utility.

## Outcome

This work demonstrates a practical strategy for real-time biopsy clip localization using co-registered photoacoustic and ultrasound imaging. The PAUSIV platform showed strong performance in both ex vivo and in vivo studies, including cases where ultrasound alone provided limited clip visibility. By combining multimodal imaging with deep-learning-based detection, this project highlights the potential of PAUSIV to reduce reliance on conventional localization procedures and improve image-guided breast cancer surgery.
