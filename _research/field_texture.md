---
layout: page
title: Text-Guided 3D Texture Generation
description: Generating photorealistic textures for 3D objects from text prompts
img: /assets/research/image/texture.png
importance: 5
category: research
related_publications: false
---

## 🎬 Project Overview

<video width="100%" controls style="margin: 20px 0;">
  <source src="/assets/research/video/Introduce_texture.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

> This project explores how to generate high-quality, photorealistic textures for 3D objects using natural language prompts and diffusion models.

---

## ❌ Limitations of Baseline (TEXTure)

<video width="100%" controls style="margin: 20px 0;">
  <source src="/assets/research/video/texture_paper_result.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

> The baseline model, **TEXTure**, struggles with **viewpoint inconsistency**—textures generated from different views do not align well, leading to visual artifacts and unrealistic appearance in 3D space.

---

## 🔧 Our Approach

<img src="/assets/research/image/texture_piepeline.png" alt="Texture Pipeline" style="width:100%; margin: 20px 0; box-shadow: 0 0 8px rgba(0,0,0,0.1); border-radius: 8px;">

To overcome the limitations of TEXTure, our method introduces the following improvements:

- **Multi-view 2×2 grid** is applied during both training and inference to **enforce texture consistency** across views.
- **Stable Diffusion 1.5 → SDXL**: We replace the backbone with **Stable Diffusion XL**, which improves texture fidelity and detail.
- **Delighting module** is integrated to remove lighting inconsistencies across views, yielding more coherent and photorealistic results.

---
