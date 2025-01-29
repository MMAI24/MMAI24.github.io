---
layout: page
title: 3D Human Vision & Graphics
description: 3D human pose estimation and tracking, NeRF-based novel view and pose rendering for human
img: /assets/img/body2.jpg
importance: 3
category: research
related_publications: true
---

Creating high-fidelity human avatars is a significant topic in metaverse, AR and VR applications. To achieve this, various solid algorithms are necessary, including 3D human body and pose reconstruction, generation, and realistic rendering. During in Microsoft Research Asia, PI contributed to multiple projects focused on these topics {% cite gaoMPSNeRFGeneralizable3D2022a %}, {% cite kimMNETMusicDrivenPluralistic2023 %}, {% cite kimImplementationOmnidirectionalHuman2015 %}.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/sl_data.png" title="example image" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    Human pose tracking of sign language videos. Accurate human body and hand pose tracking with weakly synchronized multi-view videos.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/mnet_generation_diversity.png" title="example image" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    Dance motion generation conditioned on various music sequences.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/mps_pipeline.png" title="example image" class="img-fluid" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/mps_teaser.png" title="example image" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    MPS-NeRF. Model & pose agnostic NeRF-based human rendering.
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/img/research/mpsnerf_demo.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    MPS-NeRF demo videos
</div>
