# Pneumonia-Diagnosis-using-XRays





## **Summary**

The risk of pneumonia is immense for many, especially in developing nations where billions face energy poverty and rely on polluting forms of energy. The WHO estimates that over 4 million premature deaths occur annually from household air pollution-related diseases including pneumonia. In such regions, the problem can be further aggravated due to the dearth of medical resources and personnel. For example, in Africa’s 57 nations, a gap of 2.3 million doctors and nurses exists. For these populations, accurate and fast diagnosis means everything. It can guarantee timely access to treatment and save much needed time and money for those already experiencing poverty.

This project is about diagnosing pneumonia from XRay images of lungs of a person using self laid convolutional neural network. My work includes self laid neural network which was repeatedly tuned for one of the best hyperparameters and used variety of utility function of keras like callbacks for learning rate reduction and checkpointing. Data augmentation was used for a better modelling. Other metrics like precision , recall and f1 score using confusion matrix were taken off special care. 





## **Data Source**

In this case, using x-ray images of pediatric patients to identify whether or not they have pneumonia. The dataset comes from Kermany et al. on [Mendeley](https://data.mendeley.com/datasets/rscbjbr9sj/3), although there is also a smaller version on [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).





## **Language and Packages Used**

* import os
* import numpy as np
* import pandas as pd 
* import random
* import cv2
* import matplotlib.pyplot as plt
* import keras.backend as K
* from keras.models import Model, Sequential
* from keras.layers import Input, Dense, Flatten, Dropout, BatchNormalization
* from keras.layers import Conv2D, SeparableConv2D, MaxPool2D, LeakyReLU, Activation
* from keras.optimizers import Adam
* from keras.preprocessing.image import ImageDataGenerator
* from keras.callbacks import ModelCheckpoint, ReduceLROnPlateau, EarlyStopping
* import tensorflow as tf
* import skimage
* from skimage.transform import resize





