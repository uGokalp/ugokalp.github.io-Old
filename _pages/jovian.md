---
layout: archive
title: "Jovian project"
permalink: /jovian/
github: "https://github.com/uGokalp/ML-in-Numpy"
author_profile: true
---


## My Jovian ZerotoGANs Submission

For my project I've decided to do a project on fruit classification which I hope to later use in a object detection application.

The dataset is from https://www.kaggle.com/moltean/fruits.

Originaly the data had 131 different fruits and vegetables but I've reduced it to 51 to utilize more data per fruit.

[Link to my submission](https://jovian.ml/ugokalp/final-project)

### DataLoader

Since the dataset was already organized into subfolders with each folder named after the class name I've decided to use ImageFolder from torchvision.datasets. This greatly simplified the process.


I've decided to use 32 for the batch size. (see. https://twitter.com/ylecun/status/989610208497360896?lang=en)

Since the data already had transformations such as rotation and flips, I did not apply any special transformations.

Entire set: 32316
Train set: 24,237
Valid set: 8079

1/4 of the entire dataset(8079) was used for validation.

### Measuring Performance

The dataset was fairly evenly distributed with most classes more than 450 observations. For that reason I only tracked loss and accuracy.

## Best Model

The best model was the model discussed in the lectures, with 6 convolutional layers from 3 to 256 feature maps with batch normalization after every convolutional layers and 2 linear layers.

To train the model OneCycleLR scheduler along with Adam optimizer and Cross Entropy loss was used.

Best model was found after testing 2 different architectures with varying learning rates.

The model reaches 100% accuracy with minute loss after 5 epochs with a learning rate of 0.01.


# Thank you to Aakash N S for this course.


