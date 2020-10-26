---
title: "Document Dewarp"
date: 2020-05-10T01:57:14+08:00
draft: false
author: "rlee"
summary: "We treat document dewarp as an end-to-end dense labeling problem and adopt Neural Architecture Search to find the best model."
reading_time: true  # Show estimated reading time?
share: false  # Show social sharing links?
profile: true  # Show author profile?
commentable: true  # Allow visitors to comment? Supported by the Page, Post, and Docs content types.
---

The ubiquity of hand holding devices have led to more and more document images being captured by mobile cameras instead of scanned, which helps the digitization of document image more accessible to people. Once captured, the digitized document can be used for further processing and analysis. While taking the images of document, it is desired that the characters and patterns on the document being preserved with best possible accuracy. However, photographed documents are often folded or crumpled in an unconstrained environment, thus unsuitable for document information extraction using Optical Character Recognition (OCR) and other methods, whose accuracy suffered significant loss because of geometric distortions. As a result, it is thus desirable for the original images taken by camera being rectified using preprocessing technique, which helps narrow the quality gap between photographed document and scanned document. 

In our work, we apply deep learning method to tackle this problem. Comparing to previous work, we focus on two motivations: 1. Find out what ground truth information is necessary for the precise regress of coordinate mapping. 2. Using the given ground truth information, find the neural network architecture with the best accuracy. Towards our two targets, we designed a novel neural architecture search method, which can automatically choose the supervision information needed and search for the best neural architecture. Not only did we evaluate our method on multiple open-source document dewarp dataset to prove the efficiency of our method, but also we expand the variety of dataset with more 3D warped paper models using Blender. 
