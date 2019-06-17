# Food Classification with Deep Learning in Fast.ai

## Overview
Food-101 is a challenging data set of 101 food categories, with 101'000 images. For each class, 250 manually reviewed test images are provided as well as 750 training images.

The purpose of this project is to create a deep learning model to classify images using the Fast AI library and the Food-101 dataset. The created model aims to get close to matching some recent state of the art results. The target is >85% for top-1 accuracy.

## Dataset
### Food-101 Dataset
**Source** - https://www.vision.ee.ethz.ch/datasets_extra/food-101/
### Dataset Description
Total 101,000 images<br>
101 food categories<br>
1000 images for each category - 750 training images and 250 test images

## Dependencies
Install the following dependencies using pip
* matplotlib
* fastai
* pandas

## Result
Top-1 and Top-5 accuracy are used for evaluating the model.
### Results on dataset 
* **Top-1** - 86.72%
* **Top-5** - 96.99%

## Possible Improvements
* Only basic transformations were used in this model. Possible enhancements would be to try other augmentations like jitter or skew. Also, the brightness and contrast parameters would be tuned for a higher range. This might help with separating food dishes that have similar color, but different shapes - or similar shapes with different colors.
* A deeper ResNet model could be used to improve the result at the cost of the size of a larger model and more computation time.