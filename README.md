# Image-Colorization-of-Historical-Paintings

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Y0uwtnjP9eA-YGim1RlEXdkPIGaZAUcF)

### Introduction

&nbsp;&nbsp;&nbsp;Colorization and remastering of old images nowadays is usually done manually by using popular photo editing software like <b>Photoshop</b>. This process is generally a very demanding job that requires extensive research, in order to properly organize the layers of color as well as the proper shading of these images. Sometimes remastering an image can take months. However, with the help of various <b> Deep Learning </b>models it is possible to gradually speed up and even automate this task, whilst producing results that would be similar to those of a professional editor.   

### Motivation
&nbsp;&nbsp;&nbsp;My personal goal for this research was to gain more experience in preprocessing, training, optimizing and evaluating <b>Image-related neural networks</b>. In my previous projects, I have mostly gravitated towards classification tasks, so I have decided to step a little bit further into the field of <b>Generative models</b>. The main reason for that is the fact that they produce unique results, which can be easily compared with their original counterparts and can be interpreted using visualizations instead of different performance metrics.


### Problem statement

&nbsp;&nbsp;&nbsp; This project is basically just me reproducing F. Baldasarre's paper on [Image Colorization using CNN's and ResNet](https://arxiv.org/pdf/1712.03400.pdf) and following E. Wallner's [tutorial](https://medium.freecodecamp.org/colorize-b-w-photos-with-a-100-line-neural-network-53d9b4449f8d) on this task with some adjustments in terms of the data, preprocessing and training parameters. My main goal is to try to <b>recolorize</b> images of famous painters, which are previously converted to <b>grayscale</b>. After the testing step, I will also try to colorize some images that were originally black-and-white and see how the model performs there.

### Datasets
&nbsp;&nbsp;&nbsp; The main dataset for this project is the resized (smaller) version of [Best Artworks of All Time](https://www.kaggle.com/ikarus777/best-artworks-of-all-time), downloaded from <b>Kaggle</b>. It contains over <b>8000</b> images of paintings from <b>50</b> different artists. Due to time constraints, however, I will only be using <b>2500</b> of those images for training.

&nbsp;&nbsp;&nbsp; I am also indirectly using the widely-popular [ImageNet dataset](http://www.image-net.org/), due to the fact that a pre-trained <b>Inception-Resnet-v2</b> model is applied to the main model for feature extraction. 

### Main Libraries

*   <b>Numpy</b> - mainly for storing images as features
*   <b>Matplotlib</b> - visualizing results and model performance
*   <b>Scikit-image</b> - image transformations, reading and plotting
*   <b>Scikit-learn</b> - model data splitting
*   <b>Tensorflow (Keras API)</b> - creating, optimizing, saving and preprocessing deep learning models

&nbsp;&nbsp;&nbsp; This project is also made entirely on <b>Google Colab</b> for performance sake.

