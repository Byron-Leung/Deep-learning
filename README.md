# Deep-learning
￼


model_script.py

Overview
This model script has been trained by a large data set contains 120 different classes.
The final training accuracy goes over 95% and validation accuracy over 70% totally.

Dataset
The Stanford Dogs dataset contains 20580 images of 120 breeds of dogs from around the world and each breed has around 170 images on average.
* “Images” directory: Images files (JPG) of different breeds are stored in a separate folder which named by its breed id and name (e.g. n02085620-Chihuahua). Images in each folder are named by breed id followed by image id.
* “Annotation” directory: Same structure with “Images” directory that each image has a corresponding annotation. It contains the class label of image, image size and the coordinate of bounding box which indicates the location of dog in the image.
* “list” directory: Including file_list.mat, train_list.mat and test_list.mat which is the list of all files, training images and test images in the datasets respectively. 
Linux Terminal Instructions
This script requires python 2.7+.


1. The following libraries must be installed locally:
* Keras
* Split_folders
* ImageDataGenerator from keras.preprocessing.image
from keras.models import Sequential
from keras.layers import Dense, Dropout, Flatten
from keras.layers import Conv2D, MaxPooling2D
from keras import models
from keras import layers
from keras.applications.vgg16 import vgg16
from keras import optimizers
import matplotlib.pyplot as plt
from keras.utils import plot_model
from keras.models import load_model
from keras.applications.xception import xception
from keras.utils.np_utils import to_categorical
from sklearn.metrics import confusion_matrix
from keras.models import load_model
import matplotlib.pyplot as plt
import itertools
import sklearn.metrics as metrics
import numpy as np
pandas

2. Use cd command to move to the directory where the script is located.

3. Before running the script from terminal, make sure that all the data frames (train, development and test) are saved in the same directory as the file.

4. Type the python version installed in your system followed by the name of the script, including the extension .py (i.e. python3 model_script.py).

5. The model will take a long time to run, ouput a lot of figures and its corresponding results.
