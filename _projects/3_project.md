---
layout: page
title: Sparse-view 3D Reconstruction using Gaussian Splatting
description: Variance Sampling Strategy for efficient reconstruction
img: assets/img/preview.gif
importance: 3
category: work
---


We compared the performance of NeRF with and without SDS guidance from the diffusion to model to see the impact for different number of input views. (The ZeroNVS paper only compares performance for a single view of a scene)

Our focus is on improving the view selection for SDS so that we can maximize the performance boost for lesser number of input views (<25).

The ZeroNVS algorithm currently randomly samples views around the object (6 views per iteration) and the views are randomly noised with the object masked using depth from NeRF so that foreground is not learnt using SDS.

The variance sampling strategy reduces the number of views sampled by filtering them out based on variance of the CLIP embedding of the RGB samples.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/psnr.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ssim.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lpips.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Quantitative Results for View Selection using Variance Sampling Strategy
</div>


<div class="col-sm mt-3 mt-md-0">
{% include video.liquid loading="eager" path="assets/img/baseline.mp4" title="example image" class="rounded z-depth-1" autoplay='true'%}
</div>
<div class="caption">
    Baseline Reconstruction using ZeroNVS
</div>

<div class="col-sm mt-3 mt-md-0">
{% include video.liquid loading="eager" path="assets/img/SDS.mp4" title="example image" class="rounded z-depth-1" autoplay='true'%}
</div>
<div class="caption">
    Reconstruction using Scored Distillation Sampling
</div>

<div class="col-sm mt-3 mt-md-0">
{% include video.liquid loading="eager" path="assets/img/sds_var_samp.mp4" title="example image" class="rounded z-depth-1" autoplay='true'%}
</div>
<div class="caption">
    Reconstruction using Variance Sampling Strategy
</div>





