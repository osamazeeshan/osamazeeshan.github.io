<!-- ---
layout: publication
title: Progressive Multi-Source Domain Adaptation
bibtex_key: zeeshan2025progressive
--- -->

# Bringing Personalization to Facial Expression Recognition

### Progressive Multi-Source Domain Adaptation (P-MSDA)

**Based on our publication in *IEEE Transactions on Affective
Computing***

Facial Expression Recognition (FER) is becoming a crucial component in
many real-world systems --- from driver monitoring and clinical pain
assessment to intelligent tutoring and human--computer interaction. Yet
even with today's deep learning models, a major challenge persists:

> **People express emotions differently.**

Variations in age, gender, ethnicity, facial structure, and even camera
conditions cause models to fail when deployed on a new person.

This makes **personalized FER** essential. However, most methods either
require labeled personal data (which is impractical) or fail to
generalize due to large domain shifts between individuals.

In our recent work, we introduce **Progressive Multi-Source Domain
Adaptation (P-MSDA)** --- a curriculum-inspired strategy that adapts a
model to a new, unlabeled target individual progressively.

------------------------------------------------------------------------

## 🔍 Problem Overview

Multi-source domain adaptation (MSDA) assumes using **all available
subjects** as sources will make the model more robust. Surprisingly, our
analysis shows this is not true.

-   Some source subjects differ drastically from the target.
-   Many introduce **negative transfer**.
-   Using all sources increases computational cost without improving
    generalization.

> **Some source subjects help adaptation, but many make it worse.**

------------------------------------------------------------------------

## 💡 Our Solution: Progressive MSDA (P-MSDA)

P-MSDA learns from source subjects *in a progressive, similarity-based
sequence*.

### ✔ Subject Ranking Based on Similarity

We compute cosine similarity between deep feature embeddings and rank
all source subjects relative to the target.

### ✔ Progressive Adaptation

Adaptation begins from the most similar source, adding new subjects one
at a time.\
This reduces domain shift early and stabilizes learning.

### ✔ Density-Based Replay Memory

We maintain a replay buffer using DBSCAN-based density estimation to
retain only the **most representative samples**.

### ✔ Domain Alignment with MMD

We minimize discrepancy across: - Current source domain\
- Replay memory\
- Target domain

Yielding a unified, target-aligned feature space.

------------------------------------------------------------------------

## 📈 Results Across Benchmark Datasets

Evaluated on BioVid, UNBC-McMaster, Aff-Wild2, and BAH:

### 🟦 BioVid Pain Dataset

-   **88% accuracy**, outperforming all state-of-the-art baselines.
-   In some subjects, P-MSDA nearly matches supervised Oracle
    performance.

### 🟩 UNBC-McMaster

-   **0.88 accuracy**, significantly higher than existing adaptation
    methods.

### 🟨 In-the-Wild (Aff-Wild2, BAH)

Despite severe real-world noise:

-   Aff-Wild2: **0.46**
-   BAH: **0.71**

Both significantly outperform MSDA baselines.

### 🟥 Cross-Dataset (UNBC → BioVid)

-   P-MSDA achieves **0.78 accuracy**, confirming robustness under
    extreme domain shift.

------------------------------------------------------------------------

## 🎯 Why It Works

Ablation studies show:

-   **Curriculum ordering** is essential.
-   **Density-based replay sampling** ensures high-quality knowledge
    retention.
-   **Progressive alignment** yields compact, target-specific feature
    clusters.
-   **Efficient training**: only 3 domains are used at any time.

------------------------------------------------------------------------

## ✨ Takeaway

P-MSDA enables:

-   Personalized FER **without labeled target data**
-   Scalable multi-subject adaptation
-   Avoidance of negative transfer
-   State-of-the-art performance across multiple datasets

This is a step toward practical FER systems in healthcare, education,
HCI, and affective computing.

------------------------------------------------------------------------

## 📄 Full Paper

**Title:** Progressive Multi-Source Domain Adaptation for Personalized
Facial Expression Recognition\
**Authors:** Muhammad Osama Zeeshan, Marco Pedersoli, Alessandro L.
Koerich, Eric Granger\
**Venue:** IEEE Transactions on Affective Computing

------------------------------------------------------------------------

## 📬 Contact

Feel free to reach out for collaboration or questions!
