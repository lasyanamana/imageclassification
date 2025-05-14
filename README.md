# Image Classification using Convolutional Neural Network (CNN)

## Project Overview
This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images from the CIFAR-10 dataset. The model achieves approximately 70-75% accuracy on the test set.

## Dataset
**CIFAR-10 Dataset**:
- 60,000 32x32 color images
- 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- 50,000 training images
- 10,000 test images

## Model Architecture
```python
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d (Conv2D)             (None, 30, 30, 32)        896       
                                                                 
 max_pooling2d (MaxPooling2D  (None, 15, 15, 32)       0         
 )                                                               
                                                                 
 conv2d_1 (Conv2D)           (None, 13, 13, 64)        18496     
                                                                 
 max_pooling2d_1 (MaxPooling  (None, 6, 6, 64)         0         
 2D)                                                             
                                                                 
 conv2d_2 (Conv2D)           (None, 4, 4, 64)          36928     
                                                                 
 flatten (Flatten)           (None, 1024)              0         
                                                                 
 dense (Dense)               (None, 64)                65600     
                                                                 
 dense_1 (Dense)             (None, 10)                650       
                                                                 
=================================================================
Total params: 122,570
Trainable params: 122,570
Non-trainable params: 0
Requirements
Python 3.7+

TensorFlow 2.x

NumPy

Matplotlib

scikit-learn

Seaborn
Usage
Run all cells in the notebook sequentially

The notebook will:

Download and preprocess the CIFAR-10 dataset

Build and train the CNN model

Evaluate performance on test data

Generate visualizations of results

Results
Typical performance metrics:

Test Accuracy: ~70-75%

Training Time: ~5-10 minutes on CPU
