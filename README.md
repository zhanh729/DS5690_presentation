# DS5690_presentation
## BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation

This document synthesizes the insights from the research paper "BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation," detailing a novel framework for enhancing the performance of vision-language models by refining the quality of training data through a bootstrapping method known as CapFilt.

Presenter: Haonan Zhang, Zhenyu Liu

## Overview
---
The BLIP framework integrates a new approach to pre-train a vision-language model by leveraging a bootstrapped dataset, which enhances the model's performance across various downstream tasks by refining the noisy web-collected image-text pairs, aiming to bridge the gap between large-scale noisy web data and the need for high-quality training sets. The document outlines the BLIP's solution to these issues, highlighting its unique bootstrapping process that leads to improved model performance across a variety of tasks.

### Introduction
While existing vision-language models demonstrate impressive capabilities, they often require extensive data and compute resources. BLIP
addresses this by introducing a novel bootstrapping method called CapFilt, which utilizes synthetic caption generation and filtering to improve data quality for model pre-training.
