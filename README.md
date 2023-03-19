# Problem_Statement_3_Clothing-_Recognition_for_Personalized_Recommendations
This is A Deep Learning based Fashion Recommender System using the ResNET50

## Pre - Requisite :
1. Deep Learning ----> CNN (A CNN is a kind of network architecture for deep learning algorithms and is specifically used for image recognition and tasks that involve the processing of pixel data.)
2. Transfer Learning ----> ResNET (Residual Network (ResNet) is a deep learning model used for computer vision applications. It is a Convolutional Neural Network (CNN) architecture designed to support hundreds or thousands of convolutional layers.) ----> ImageNET (ImageNet is an image database organized according to the WordNet hierarchy, in which each node of the hierarchy is depicted by hundreds and thousands of images.)

## Algorithm :
### 1. Import Model - 
    We have loaded a CNN (convolutional network) model which is called ResNET Module which is a trained dataset on ImageNET.We have used this model because it is a high performing CNN Model which means it has a great accuracy.
    We have to import ResNET in this step which comes built-in in Keras module.
### 2. Extract Features - 
    We have used the CNN model to extract features. We have total 373 images in our dataset used.
    User gives an another image and we compare it to the 373 images and the closest five images are the recommendations. So somehow we have to analyze this 373 images which is a difficult task and hence we extract the features. Generally image is very big in size, our images have the resolution of (224,224,3) i.e 224x224 pixels and this much pixels into 373 is a big number. Therefore we have extracted features from each image. 
    Our ResNET model extracts the features of 373 images. When we give 373 images in ResNET it gives us a set of 2048 for every image and these 2048 are the features of the image. We have total (373,2048) features in form of a 2-D array where number of rows are total number of images in dataset and number of columns are feature for each image.
### 3. Export Features - 
    It saves the features in form of a 373x2048 matrix internally so that it can be used multiple times.
### 4. Generate Recommendations - 
    When we give another image ResNET also generates a set of 2048 features(1,2048). Now, it calculates the eucledeon distance with features of the 373 images, and the neraest five image features are the recommendations which are the output. 

## Python Libraries Used :
### Numpy -
    NumPy is a Python library used for working with arrays.
### Os -
    The OS module in Python provides functions for creating and removing a directory (folder), fetching its contents, changing and identifying the current directory, etc.
### Pickle -
    Pickle in Python is primarily used in serializing and deserializing a Python object structure. In other words, it's the process of converting a Python object into a byte stream to store it in a file/database, maintain program state across sessions, or transport data over the network.
### Tenserflow -
    TensorFlow allows you to create dataflow graphs that describe how data moves through a graph. The graph consists of nodes that represent a mathematical operation. A connection or edge between nodes is a multidimensional data array.
### Keras -
    Keras is a high-level, deep learning API developed by Google for implementing neural networks. It is written in Python and is used to make the implementation of neural networks easy.
### Streamlit -
    Streamlit is a free and open-source framework to rapidly build and share beautiful machine learning and data science web apps.
### PIL -
    PIL stands for Python Imaging Library, and it's the original library that enabled Python to deal with images.
### SkLearn -
    Scikit-learn is an open source data analysis library, and the gold standard for Machine Learning (ML) in the Python ecosystem.
### cv2 -
    cv2 is the module import name for opencv-python, "Unofficial pre-built CPU-only OpenCV packages for Python".
### tqdm -
    tqdm can help you create progress bars for data processing, training machine learning models, multi-loop Python function, and downloading data from the internet.
    
## Link for Sample Dataset :
For images used refer this link:
https://drive.google.com/drive/folders/1_vNV3xy6nGpZoI7vJZ9njw1J5EJFGy2N?usp=share_link

For sample images link:
https://drive.google.com/drive/folders/13VAZ0nWsaqTLhLEqVyHdcbxQH1xk3xrg?usp=share_link

### Note :
This file is only made for working in google colab. If you want to run it on any other option such as jupiter notebook changes may occur respectively.
