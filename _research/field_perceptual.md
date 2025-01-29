---
layout: page
title: Perceptual Image Processing
description: Image & video quality assessment, AR/VR QoE assessment
img: /assets/img/perception.jpg
importance: 4
category: research
related_publications: true
---

Digital images and videos are inevitably degraded in the process from content generation to consumption. The acquisition, transmission, scaling, format conversion, or compression of images and videos introduces various types of distortions, such as white noise, Gaussian blur, blocking artifacts, banding artifact and so on. Moreover, there are often multiple interacting distortions, which complicates the problem vastly. Since human observers are the ultimate receivers of digital images and videos, quality metrics should be designed from a human-oriented perspective.
PI is one of the first pioneers applying deep neural networks to the domain of image quality assessment
{% cite kimDeepConvolutionalNeural2017a %}, {% cite kimDeepBlindImage2017 %}, {% cite kimDeepBlindImage2018 %}, {% cite kimDeepCNNBasedBlind2019 %}, {% cite kimDeepLearningHuman2017 %}, {% cite kimDeepVideoQuality2018 %}, {% cite kimFullyDeepBlind2017 %}, {% cite kimMultipleLevelFeaturebased2018 %}, {% cite kimQualityAssessmentPerceptual2014 %}, {% cite kimQualityAssessmentPerceptual2017 %}, {% cite ohBlindDeepS3D2017 %}.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/iqa_ssim.png" width=500 title="SSIM" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    Concept of classical image quality assessment. Even when various distortions exhibit the same mean squared errors, the perceived image quality can differ significantly among them.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/deep_iqa.png" title="example image" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    Deep image quality assessment by employing pseudo ground-truth data.
</div>

