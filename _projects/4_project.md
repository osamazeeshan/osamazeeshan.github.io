---
layout: page
title: Urdu OCR
description: Optical Character Recognition system for Urdu language text with video indexing capabilities.
img: assets/img/urdu-ocr.jpg
importance: 4
category: work
---


Developed a custom Urdu OCR recogntion model using Tensorflow, achieving 88% accuracy in detecting/recognizing Urdu text from low-resolution news videos. Built a content-based video indexing system (Python, C#) for news archives, reducing search time by 60% across 10,000+ hours of footage.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/urdu_detection.jpg" title="Urdu Detection" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/arabic_detect.png" title="Arabic Detection" class="img-fluid rounded z-depth-1" %}
    </div>
    <!-- <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/urdu-ocr-3.jpg" title="Video Indexing System" class="img-fluid rounded z-depth-1" %}
    </div> -->
</div>

### Text Detection Pipeline
- Implemented region-based text detection
- Developed custom preprocessing techniques for low-resolution video frames
- Created specialized filters for Urdu text enhancement

### Recognition System
- Implemented deep learning models for text recognition
- Developed post-processing algorithms for accuracy improvement

### Video Indexing System
- Built content-based video indexing system using C#
- Implemented keyframe extraction and metadata tagging
- Created semantic querying capabilities

### Results
- 88% accuracy in Urdu text detection/recognition
- 60% reduction in search time across 10,000+ hours of footage
- Published in EURASIP Journal on Image and Video Processing

### Publication
[Detection and recognition of cursive text from video frames](https://link.springer.com/article/10.1186/s13640-020-00523-5)

### Technologies Used
- Python
- TensorFlow
- OpenCV
- Tesseract OCR
- Video Processing
- Deep Learning 