# Convolutional Neural Network

This repository contains a Convolutional Neural Network (CNN) implemented using TensorFlow and Keras for image classification. The model in this code is designed to classify images of cats and dogs.

## Getting Started

### Prerequisites

- Python (>=3.6)
- TensorFlow (>=2.0)
- Keras (>=2.0)
- Pandas
- Scikit-Learn

Ensure that you have these dependencies installed before running the code.

### Installation

Clone this repository to your local machine:

```bash
git clone https://github.com/VrajMalvi/Machine-Learning/tree/main/Deep%20Learning/CNN
```

# Cat vs. Dog Showdown 🐱 🆚 🐶

Welcome to the world of cat and dog classification! In this exciting journey, we'll delve into the inner workings of a Convolutional Neural Network (CNN) and witness the epic battle between our feline friends and their canine companions.

## Data Preprocessing 📸

### Preprocessing the Training Set

Our adventure begins with the training dataset. We've enlisted the powerful `ImageDataGenerator` from Keras to help us prepare for the ultimate showdown. The images are rescaled to fit our battlefield, and we've got a few tricks up our sleeves—shearing, zooming, and even a bit of horizontal flipping.

### Preprocessing the Test Set

The test dataset gets the same treatment as our training data. All images are resized to ensure an even playing field.

## Building the CNN 🛠️

### Initializing the CNN

We've forged a mighty weapon in the form of a sequential model, utilizing TensorFlow and Keras. The quest to distinguish cats from dogs has begun!

### Step 1 - Convolution

Our first weapon is a convolutional layer with 32 filters, each with a (3,3) kernel. The ReLU activation function provides the necessary power. For colored images, the input shape is set as (64, 64, 3).

### Step 2 - Pooling

To streamline our journey, we employ a max-pooling layer with a pool size of 2 and strides of 2.

### Adding a Second Convolutional Layer

Without hesitation, we add another convolutional layer. It's so sharp that it doesn't require explicit input shape—magic, isn't it? This layer is backed up by a trusty max-pooling sidekick.

### Step 3 - Flattening

The terrain changes, and we must adapt. The model flattens, preparing for more action-packed layers.

### Step 4 - Full Connection

Our neural hero adds a dense layer with 128 units and a ReLU activation function.

### Step 5 - Output Layer

The climax approaches as we add the final dense layer. With a single unit and the power of sigmoid activation, it's ready for the ultimate binary classification showdown.

## Training the CNN 🏋️‍

### Compiling the CNN

Before we send our model into the battlefield, we equip it with 'adam'—a formidable optimizer. For victory or defeat, we've chosen 'binary_crossentropy' as our weapon. Our guiding star, 'accuracy,' will light the way.

### Training the CNN

With banners flying, the model marches onto the training set and then proceeds to face its trial on the test set. A grand total of 25 epic epochs await us!

## Making a Single Prediction 🧙‍

As the dust settles, we venture to make a single prediction. An image, whether of a cat or dog, is loaded and prepared for its fate. As the curtain falls, the class indices of 'cats' and 'dogs' reveal themselves. If the prediction is 1, it's a 'dog,' or else, it's a 'cat.'

Prepare for an adventure of pixelated proportions as we embark on this thrilling cat versus dog classification journey! 🐾✨