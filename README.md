# DS5690_presentation
## BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation

This document contains a comprehensive analysis based on the paper "BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation."

Presenter: Haonan Zhang, Zhenyu Liu


### Overview
The BLIP framework integrates a new approach to pre-train a vision-language model by leveraging a bootstrapped dataset, which enhances the model's performance across various downstream tasks by refining the noisy web-collected image-text pairs.

### Introduction
While existing vision-language models demonstrate impressive capabilities, they often require extensive data and compute resources. BLIP
addresses this by introducing a novel bootstrapping method called CapFilt, which utilizes synthetic caption generation and filtering to improve data quality for model pre-training.
