---
layout: page
title: High-Resolution Photoacoustic Microscopy System Development
description: Optical, hardware, and control development of a high-resolution PAM platform with ongoing phantom and animal imaging
img: assets/img/PAM_system.png
importance: 7
category: work
related_publications: false
---

## Project Overview

This project focuses on the development of a high-resolution photoacoustic microscopy (PAM) system designed for sensitive visualization of fine anatomical and microvascular structures. The system integrates optical excitation, ultrasound detection, hardware synchronization, and software control into a unified imaging platform for preclinical imaging applications.

A major goal of this work is to build a robust and flexible PAM system that supports high-resolution imaging while maintaining stable signal acquisition and reliable scan control. To achieve this, I worked on the optical path design, hardware integration, LabVIEW-based system control, and system-level calibration. The platform is currently being used for phantom and animal imaging studies to evaluate image quality, contrast performance, and biological imaging capability.

Overall, this project represents a combination of instrumentation development and imaging validation, with an emphasis on building a practical high-resolution PAM platform for biological and preclinical applications.

## What I Did

In this project, I worked on the design and integration of the PAM system, including the optical path, ultrasound detection setup, hardware synchronization, and LabVIEW control framework. I developed the control workflow for system operation and coordinated the timing of acquisition components to support stable and repeatable imaging.

I also performed system calibration and implemented jitter correction to improve acquisition consistency and signal reliability. In parallel, I optimized scanning protocols for high-resolution imaging of fine structures. The system has now progressed from instrumentation development into phantom and animal data acquisition for further validation.

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/hardware.png" title="Overall PAM system" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overall high-resolution photoacoustic microscopy system, showing the integrated hardware platform for imaging, detection, and acquisition.
</div>

<div class="row justify-content-center">
    <div class="col-sm-8 mt-4 mt-md-0">
        {% include figure.liquid path="assets/img/optical_path.png" title="Optical path design" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Optical path design of the PAM system, illustrating laser delivery, beam guidance, and alignment for high-resolution photoacoustic excitation.
</div>

<div class="row justify-content-center">
    <div class="col-sm-8 mt-4 mt-md-0">
        {% include figure.liquid path="assets/img/labview.png" title="LabVIEW control and acquisition framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    LabVIEW-based control and synchronization framework for scan execution, hardware coordination, and data acquisition.
</div>

## System Design and Control

The PAM platform was developed as an integrated imaging system in which optical excitation, acoustic detection, and scan control must operate in a coordinated and stable manner. I worked on the optical path setup to ensure proper light delivery to the imaging target and integrated the high-resolution probe with the rest of the acquisition hardware.

A key part of the project was building the LabVIEW control framework for synchronized operation of the imaging system. This included coordinating hardware timing, scan execution, and acquisition flow so that the platform could support reliable and repeatable imaging experiments.

## Calibration and Signal Stability

To improve system performance, I carried out calibration and correction steps aimed at increasing acquisition accuracy and consistency. In particular, I completed system jitter correction and calibration to improve timing stability and reduce variability across scans. These steps were important for maintaining image quality and enabling robust interpretation of high-resolution PAM data.

This calibration work established a more stable foundation for subsequent phantom and animal experiments and helped transition the system from development stage to practical imaging use.

## Current Imaging Studies

The project has now advanced to phantom and animal imaging for evaluation of system capability and imaging performance. These studies are being used to assess resolution, contrast, and sensitivity in representative biological and preclinical settings.

By moving from system construction to real experimental imaging, this work is helping validate the practical utility of the PAM platform and identify opportunities for further optimization in both instrumentation and imaging workflow.

## Why It Matters

High-resolution photoacoustic microscopy provides a powerful way to visualize fine biological structures with optical absorption contrast, but achieving reliable performance requires careful integration of optics, hardware, control, and calibration. A well-designed PAM system must not only provide high spatial resolution, but also maintain stable acquisition and reproducible scanning in practical imaging experiments.

This project addresses those challenges by combining system engineering with experimental validation. It contributes to the development of a robust PAM platform for biological and preclinical imaging and supports future applications that require sensitive visualization of microvascular and tissue features.

## Outcome

This project established a high-resolution PAM platform that integrates optical path design, hardware development, LabVIEW-based control, and system calibration. I completed jitter correction and calibration to improve acquisition stability and have advanced the system to phantom and animal imaging studies. Overall, this work provides a strong foundation for continued development and application of high-resolution PAM in preclinical imaging.
