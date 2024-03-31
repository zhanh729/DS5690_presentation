Algorithm: CapFilt Process in BLIP Framework

/* Applies CapFilt to enhance the dataset quality by generating synthetic captions and filtering noisy data, pre-training models for image-text tasks */

Input: image_dataset (set of images), pre_trained_model (pre-trained vision-language model), capfilt_model (CapFilt model with captioner and filter)
Output: enhanced_dataset (quality-enhanced set of image-text pairs)

1. For each image in image_dataset:
   
    a. Generate original captions using the pre_trained_model.
   
    b. Generate synthetic captions using the captioner component of the capfilt_model.
   
    c. Evaluate both original and synthetic captions using the filter component of the capfilt_model, removing noisy captions.

// Execute the CapFilt process

2. Initialize enhanced_dataset as an empty list.
   
3. For each pair of captions (original and synthetic):
   
    a. For each synthetic_caption:
   
        i. If the filter assesses the synthetic_caption as non-noisy, retain it.
   
        ii. Otherwise, remove the synthetic_caption from the dataset.
   
    b. Combine the retained synthetic captions with the original captions to form the enhanced_dataset.

5. Return the enhanced_dataset, which will be used to pre-train a new model with improved data quality.
