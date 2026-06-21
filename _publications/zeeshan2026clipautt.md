---
layout: publication
title: CLIP-AUTT: Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition
bibtex_key: zeeshan2026clipautt
---

<div class="text-center my-4">
  <h1 class="post-title">CLIP-AUTT</h1>
  <h3 class="font-weight-normal">Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition</h3>
  <p class="lead mt-3">
    Muhammad Osama Zeeshan · Masoumeh Sharafi · Benoît Savary · Alessandro Lameiras Koerich · Marco Pedersoli · Eric Granger
  </p>
  <p class="h5"><strong>ECCV 2026: The 19th European Conference on Computer Vision, Malmö, Sweden</strong></p>
  <p class="mt-3">
    <a class="btn btn-sm z-depth-0" href="https://arxiv.org/pdf/2603.27999" role="button">PDF</a>
    <a class="btn btn-sm z-depth-0" href="#citation" role="button">Citation</a>
  </p>
</div>

---

{% include figure.liquid loading="eager" path="assets/img/publications/CLIP-AUTT.png" class="img-fluid rounded z-depth-1" %}

## Overview

CLIP-AUTT focuses on **fine-grained video emotion recognition** for subtle, subject-specific expressive patterns. It brings together vision-language representations, facial Action Unit (AU) semantics, and test-time personalization so that emotion recognition models can adapt to unseen subjects without requiring labeled target data.

## Abstract

Personalized emotion recognition is important for interpreting subtle expressions that vary across individuals. CLIP-AUTT uses **Action Units as structured text prompts** inside CLIP, allowing the model to capture localized and interpretable facial cues instead of relying on noisy generated text prompts or expensive language-model supervision.

The work first introduces **CLIP-AU**, an AU-guided temporal learning approach for learning subject-agnostic facial dynamics. It then extends this formulation to **CLIP-AUTT**, a test-time personalization method that adapts AU prompts for videos from unseen subjects while preserving temporal consistency.

## Method

CLIP-AUTT is built around three core ideas:

1. **AU-guided prompting:** Action Units provide interpretable semantic prompts that describe fine-grained facial muscle activations.
2. **Temporal emotion modeling:** Video-level temporal information is used to capture gradual, subtle changes in expression.
3. **Test-time personalization:** Entropy-guided temporal window selection and prompt tuning adapt the model to subject-specific expression patterns at inference time.

## Results

The method is evaluated on three challenging video-based subtle emotion recognition datasets:

- **BioVid** for pain-related expression analysis.
- **StressID** for stress recognition.
- **BAH** for ambivalence/hesitancy recognition in behavioral-change videos.

Across these settings, CLIP-AU and CLIP-AUTT improve robustness and personalization for subtle emotion recognition compared with state-of-the-art CLIP-based facial expression recognition and test-time adaptation methods.

## Takeaway

CLIP-AUTT shows that AU-based prompt personalization can make CLIP-style video emotion recognition more interpretable, temporally consistent, and subject-aware. This is especially relevant for real-world human behavior analysis, where expressions are subtle and vary strongly across individuals.

## Paper Details

**Title:** CLIP-AUTT: Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition

**Authors:** Muhammad Osama Zeeshan, Masoumeh Sharafi, Benoît Savary, Alessandro Lameiras Koerich, Marco Pedersoli, Eric Granger

**Venue:** ECCV 2026: The 19th European Conference on Computer Vision, Malmö, Sweden

🔗 **Read the paper:** [PDF](https://arxiv.org/pdf/2603.27999)

---

## Citation {#citation}

```bibtex
@inproceedings{zeeshan2026clipautt,
  title={CLIP-AUTT: Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition},
  author={Zeeshan, Muhammad Osama and Sharafi, Masoumeh and Savary, Beno{\^i}t and Koerich, Alessandro Lameiras and Pedersoli, Marco and Granger, Eric},
  booktitle={ECCV 2026: The 19th European Conference on Computer Vision, Malmö, Sweden},
  year={2026}
}
```

## Contact

Feel free to reach out for discussion or collaboration.
