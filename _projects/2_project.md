---
layout: page
title: Model-Based Deep Learning for 3D Linear-Array PACT
description: Improving 3D photoacoustic imaging with multiview acquisition and deep learning
img: assets/img/Multiview_DL_network.png
importance: 2
category: work
giscus_comments: false
---

This project focuses on improving the three-dimensional imaging performance of linear-array photoacoustic computed tomography (PACT), which commonly suffers from poor elevational resolution compared with its axial and lateral resolution. It is based on our work (under review) in *IEEE Transactions on Biomedical Engineering (TBME)* {% cite miao_underreview_isotropic %}. To address this limitation, we developed **MV-FISTA-Net**, a model-based deep learning framework that combines multiview acquisition with learnable iterative reconstruction. By integrating complementary information from multiple scanning views, this method enhances spatial resolution and improves the fidelity of volumetric photoacoustic imaging.

A key component of this work is the multiview deep learning reconstruction framework. MV-FISTA-Net extends the conventional FISTA-based multiview deconvolution approach into a learnable 3D architecture, allowing the network to recover high-frequency information lost in conventional single-view or purely iterative reconstruction methods. This design improves image sharpness while maintaining structural consistency across the reconstructed volume.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Multiview_DL_network.png" title="MV-FISTA-Net architecture" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Overview of the MV-FISTA-Net framework for multiview photoacoustic reconstruction.
</div>

To improve generalization, we employed a two-stage training strategy. The model was first pretrained on synthetic datasets to learn the deblurring and reconstruction task under fully supervised conditions, and was then fine-tuned using a mixture of synthetic and experimental data to better adapt to real imaging conditions. This approach enables the network to preserve high-resolution priors while accounting for system-specific blurring and experimental variability.

The proposed method was validated on simulation, phantom, and in vivo human datasets. Results demonstrated that MV-FISTA-Net provides improved elevational resolution compared with both single-scan reconstruction and conventional multiview iterative reconstruction. In addition, the method significantly reduces inference time, supporting its potential for practical high-resolution 3D photoacoustic imaging applications.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Multiview_DL_example.png" title="In vivo wrist imaging result" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Representative in vivo human imaging results showing improved vascular delineation with MV-FISTA-Net.
</div>

Overall, this project demonstrates a scalable strategy for achieving near-isotropic volumetric imaging in linear-array PACT by combining multiview data acquisition with model-based deep learning. It highlights the potential of computational imaging to overcome intrinsic hardware limitations and improve the clinical utility of photoacoustic tomography.
