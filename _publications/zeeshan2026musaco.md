---
layout: publication
title: MuSACo: Multimodal Subject-Specific Selection and Adaptation for Expression Recognition with Co-Training
bibtex_key: zeeshan2026musaco
---

## Leveraging Multimodality for Personalized Expression Recognition

**Published in WACV 2026: IEEE Winter Conf. on Applications of Computer Vision**

---

## 🔍 Problem Overview

Personalized expression recognition (ER) involves adapting machine learning models to subject-specific data to improve recognition of expressions with considerable inter-personal variability. While Multi-Source Domain Adaptation (MSDA) can improve robustness by treating subjects as domains, current state-of-the-art methods often overlook multimodal information or blend sources into a single domain. This limits subject diversity and fails to explicitly capture unique subject-specific characteristics.

{% include figure.liquid loading="eager" path="assets/img/publications/musaco_motiv.png" class="img-fluid rounded z-depth-1" %}

**Figure 1** compares different approaches:

 - (a) Unimodal MSDA:** Aligns sources within a single modality, which often reduces accuracy.

 - (b) Multimodal UDA (Blending):** Blends sources into a single domain, failing to exploit subject-specific diversity.

 - (c) MuSACO (Ours):** Selects relevant sources per modality using co-training and aligns them using both class-aware and class-agnostic losses.

**Existing methods often fail to generalize for subtle expressions and across diverse individuals due to variations in cultural and individual expressiveness.**