---
layout: page
title: Urdu OCR
permalink: /projects/urdu-ocr/
description: Detailed overview of the Urdu OCR project
nav: true
nav_order: 1
---

# Urdu OCR Project

## Project Overview
Developed a custom Urdu OCR pipeline using OpenCV and Tesseract, achieving 88% accuracy in detecting/recognizing Urdu text from low-resolution news videos. Built a content-based video indexing system (Python, TensorFlow) for news archives, reducing search time by 60% across 10,000+ hours of footage.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/urdu-ocr-1.jpg" title="Text Detection Pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/urdu-ocr-2.jpg" title="Recognition Results" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/urdu-ocr-3.jpg" title="Video Indexing System" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Technical Details

### Text Detection Pipeline
- Implemented region-based text detection using OpenCV
- Developed custom preprocessing techniques for low-resolution video frames
- Created specialized filters for Urdu text enhancement

### Recognition System
- Fine-tuned Tesseract OCR for Urdu language
- Implemented deep learning models for text recognition
- Developed post-processing algorithms for accuracy improvement

### Video Indexing System
- Built content-based video indexing using TensorFlow
- Implemented keyframe extraction and metadata tagging
- Created semantic querying capabilities

## Results
- 88% accuracy in Urdu text detection/recognition
- 60% reduction in search time across 10,000+ hours of footage
- Published in EURASIP Journal on Image and Video Processing

## Publication
[Detection and recognition of cursive text from video frames](https://link.springer.com/article/10.1186/s13640-020-00523-5)

## Technologies Used
- Python
- TensorFlow
- OpenCV
- Tesseract OCR
- Video Processing
- Deep Learning 