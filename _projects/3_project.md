---
layout: page
title: PAUSIV for Breast Cancer Localization
description: Real-time photoacoustic and ultrasound imaging for biopsy clip detection in breast surgery
img: assets/img/Clip_f1.png
importance: 3
category: work
giscus_comments: false
---

This project focuses on developing **PAUSIV**, a photoacoustic/ultrasound imaging platform for real-time localization of biopsy marker clips in breast cancer surgery. In breast-conserving procedures, accurate localization of non-palpable lesions remains a major challenge, and current approaches often require additional preoperative localization procedures such as wires, seeds, or tags. PAUSIV was designed to provide a wire-free, radiation-free, and workflow-compatible alternative by directly visualizing biopsy clips with high contrast during imaging. :contentReference[oaicite:3]{index=3}

A central motivation of this work is to improve surgical guidance while reducing patient burden and procedural complexity. Because titanium biopsy clips provide strong photoacoustic contrast relative to surrounding tissue, they can serve as effective intraoperative targets for localization. Our system combines photoacoustic contrast with co-registered ultrasound, enabling both structural guidance and clip-specific visualization within the same platform. :contentReference[oaicite:4]{index=4}

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Clip_f1.png" title="Ex vivo biopsy clip visualization" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Representative ex vivo breast specimen with corresponding clip localization result, demonstrating strong photoacoustic contrast of the biopsy marker clip relative to background tissue.
</div>

To support intraoperative use, the PAUSIV platform was further integrated with a deep-learning-based clip detection pipeline. The framework uses a two-stage training strategy in which ex vivo data are first used for representation learning, followed by fine-tuning on in vivo data. A vision transformer backbone with CNN-based spatial prediction was used to generate clip localization outputs, while clinical depth-note information was incorporated as a spatial prior to constrain the search region. This design improves robustness under realistic clinical variability, including differences in tissue composition, lesion depth, and patient anatomy. :contentReference[oaicite:5]{index=5} :contentReference[oaicite:6]{index=6}

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Clip_f2.png" title="Vision-language clip localization pipeline" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Overview of the vision-language pipeline for biopsy clip localization in photoacoustic images.
</div>

The system was first evaluated on ex vivo breast tissue specimens obtained in the operating room. In these studies, X-ray imaging served as the ground truth for clip location, followed by photoacoustic imaging and reconstruction. PAUSIV demonstrated strong clip conspicuity, with clip signals substantially exceeding background tissue signals and showing markedly higher contrast than ultrasound alone. In preliminary ex vivo studies involving more than 30 specimens, clip detection achieved 100% sensitivity and 100% specificity. :contentReference[oaicite:7]{index=7}

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Clip_f3.png" title="In vivo PAUSIV validation" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Representative in vivo breast imaging results showing PA, US, and PA/US overlay images. PAUSIV detected the biopsy clips across cases, including situations where ultrasound provided limited or no clip visibility.
</div>

The platform was then translated to in vivo human studies to assess clinical feasibility. Across representative breast cases, PAUSIV successfully localized biopsy clips within tumor regions, including cases where ultrasound failed to clearly visualize the embedded clip and even cases where ultrasound did not clearly show either the mass or the clip. These results demonstrate the potential of PAUSIV to complement conventional ultrasound in clinically relevant settings. :contentReference[oaicite:8]{index=8}

The real-time clip detection model also showed promising performance in vivo, with detection precision above 93%, an average processing time of 0.83 s per case, and inference speeds of approximately 30 frames per second. The model maintained stable localization across consecutive frames at depths around 30 mm, supporting its feasibility for real-time image-guided applications in breast surgery. :contentReference[oaicite:9]{index=9}

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Clip_f4.png" title="Real-time in vivo clip detection" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Real-time in vivo biopsy clip detection results, showing stable deep-tissue localization of the marker clip across consecutive photoacoustic frames.
</div>

Overall, this project demonstrates the potential of photoacoustic/ultrasound imaging to provide accurate, real-time, and clinically practical guidance for biopsy clip localization in breast cancer care. By combining hardware optimization, multimodal imaging, and deep-learning-based detection, PAUSIV offers a promising route toward reducing dependence on conventional localization procedures and improving surgical workflow.
