# VegetableFruitClassifier-Model

This repository contains the code and resources for training the Vegetable and Fruit Classifier model.

## Overview

The Vegetable and Fruit Classifier is a deep learning model based on the MobileNetV2 architecture. It is trained to classify images into various types of fruits and vegetables. The model can be used to determine the type of vegetable or fruit present in an input image.

## Dataset

The training dataset consists of a collection of labeled images of different fruits and vegetables. The dataset is organized into separate folders for each class, under different proportions of test, train and validation sets that are already organised under the dataset, the dataset can be obtained from [https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition]

## Model Training

The model training process involves the following steps:

1. Data Preprocessing: The images are preprocessed using common data augmentation techniques, such as random cropping, resizing, and normalization.

2. Model Architecture: The MobileNetV2 architecture, pre-trained on the ImageNet dataset, is used as the base model. The final classification layer is replaced to match the number of classes in the dataset.

3. Training: The model is trained using the labeled images from the dataset. The training process involves optimizing the model's parameters using a specified optimizer and loss function.

4. Evaluation: The trained model is evaluated on a separate validation set to assess its performance.

5. Model Export: Once trained, the model weights are saved for future use. The saved model is provided in the repository for quick testing of the classification model. 

## Usage

To train the Vegetable and Fruit Classifier model, follow these steps:

1. Import all the libraries included in the first cell, install the neccesary requirements provided in the requirements.txt file before running the first cell.

2. Organize your dataset into the appropriate folder structure, with separate folders for each class and under train, test and validation folders.

3. Adjust the file paths in the training script `train.py` to match your dataset directory structure.

4. Run the Training cell with epochs set according to your preference. Observe the loss function going down.

5. Run the Image classification cell after training and saving your model, provide an appropriate image source path and execute the cell and wait for it to print out the classified item. 

