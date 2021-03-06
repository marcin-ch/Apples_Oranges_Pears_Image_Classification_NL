# Apples Oranges Pears Image Classification
## Overview
Project's goal is to train 3rd party CNN (Convolutional Neural Network) for classifying images of fruits (28x28) into one of the categories:
* apple
* orange
* pear

Project has been created as Jupyter notebook hosted by Google Colaboratory (or Colab for short). Colab allows you to write and execute Python in your browser with zero configuration required, free access to GPUs and easy sharing (more info [here](https://colab.research.google.com/notebooks/intro.ipynb)).

## Notebooks explanation
* *Apples_Oranges_Pears_Image_Classification_NL.ipynb* - main functions:
  * dataset upload ([CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html)),
  * image preprocessing,
  * extracting only required classes (apple, orange, pear),
  * image cropping to 28x28 (original images are 32x32),
  * model creation, 
  * model training,
  * model saving.

  To open this notebook hit bellow button and then `Runtime -> Run All` (you must be logged in with a Google Account to continue):<br>
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/marcin-ch/Apples_Oranges_Pears_Image_Classification_NL/blob/master/Apples_Oranges_Pears_Image_Classification_NL.ipynb)

## Model saved files
* Once notebook operation is completed, new files related to model appear in the workspace (if not, please `Refresh`). It should look like as follows:<br><br>
![model_saved_files.png](https://github.com/marcin-ch/Apples_Oranges_Pears_Image_Classification_NL/blob/master/model_saved_files.PNG)<br><br>
  * *model_4layer1_FE.json* - model description
  * *model_4layer1_weights_FE.h5* - model weight values
  * *model_4layer1_full_FE.h5* - full model (weight values, model architecture, model's training configuration, the optimizer and its state, more info [here](https://www.tensorflow.org/tutorials/keras/save_and_load#hdf5_format) 
  * *model_desc_FE.txt* - model description

## Dataset
Dataset is [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html). To train the model only three classes have been used (apple, orange, pear), extraced from whole dataset. Furthermore, originally images are 32x32 and they have been changed to 28x28.
