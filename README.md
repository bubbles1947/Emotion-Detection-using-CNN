# Emotion-Detection-using-CNN


The model architecture is a standard CNN with the following structure:

4 Convolutional Blocks, each containing:

A 2D convolutional layer
Batch normalization
ReLU activation
Max pooling (reducing spatial dimensions by half each time)


Block Details:

First block: 1 → 32 channels (grayscale input to 32 feature maps)
Second block: 32 → 64 channels
Third block: 64 → 128 channels
Fourth block: 128 → 256 channels


Fully Connected Layers:

After the convolutional blocks, features are flattened
First FC layer: 256×3×3 → 512 neurons
Dropout (50%) for regularization
Final FC layer: 512 → 7 neurons (one for each emotion class)



Image Processing

Input images are 48×48 pixels (the standard size for FER-2013)
Images are converted to grayscale (single channel)
After 4 max pooling layers (stride 2), the feature maps are reduced to 3×3 in spatial dimensions.

NO AUGMENTATION YET. More Work in progress.
