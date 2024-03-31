Algorithm: Traditional VLP Process

/* Applies traditional VLP to train a model on a dataset for image-text tasks without CapFilt enhancements */

Input: image_dataset (set of images), noisy_data (set of image-text pairs with potential noise)
Output: vlp_model (trained vision-language model)

1. For each image-text pair in noisy_data:
   
    a. Directly encode the image into image_features using a vision_model.
   
    b. Directly encode the text into text_features using a language_model.

// Execute the traditional VLP training process

2. Initialize vlp_model with pre-set parameters.
   
4. For each encoded image-text pair (image_features, text_features):
   
    a. Train the vlp_model using a combination of image-text matching and language modeling objectives.
   
    b. No explicit filtering step is performed; model is exposed to the entire noisy dataset.

6. After training, evaluate vlp_model on a validation set to measure performance.

7. Return the trained vlp_model.
