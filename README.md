# Problem_Statement_3_Clothing-_Recognition_for_Personalized_Recommendations
This is A Deep Learning based Fashion Recommender System using the ResNET50

## Pre - Requisite :
1. Deep Learning ----> CNN (A CNN is a kind of network architecture for deep learning algorithms and is specifically used for image recognition and tasks that involve the processing of pixel data.)
2. Transfer Learning ----> ResNET (Residual Network (ResNet) is a deep learning model used for computer vision applications. It is a Convolutional Neural Network (CNN) architecture designed to support hundreds or thousands of convolutional layers.) ----> ImageNET (ImageNet is an image database organized according to the WordNet hierarchy, in which each node of the hierarchy is depicted by hundreds and thousands of images.)

## Plan of Attack
1. Import Model - We will use ResNET Module which is a CNN model (trained dataset)
3. Extract Features - 373 Images along with user given images will be bifurcated into 2048 features in form of (373,2048). 
4. Export Features - Saves the features in for of a matrices internally.
5. Generate Recommendations - Gives 5 nearest neighbours of the sample image inserted.

## Python Libraries Used :
### Numpy -
NumPy is a Python library used for working with arrays.
### Os -
The OS module in Python provides functions for creating and removing a directory (folder), fetching its contents, changing and identifying the current directory, etc.
### Pickle -
Pickle in Python is primarily used in serializing and deserializing a Python object structure.
### Tenserflow -
TensorFlow allows you to create dataflow graphs that describe how data moves through a graph. The graph consists of nodes that represent a mathematical operation. A connection or edge between nodes is a multidimensional data array.
### Keras -
Keras is a high-level, deep learning API developed by Google for implementing neural networks. It is written in Python and is used to make the implementation of neural networks easy.
### Streamlit -
Streamlit is a Python-based library that allows data scientists to easily create free machine learning applications.

For images used refer this link:
https://drive.google.com/drive/folders/1_vNV3xy6nGpZoI7vJZ9njw1J5EJFGy2N?usp=share_link

For sample images link:
https://drive.google.com/drive/folders/13VAZ0nWsaqTLhLEqVyHdcbxQH1xk3xrg?usp=share_link

### Note :
This file is only made for working in google colab. If you want to run it on any other option such as jupiter notebook changes may occur respectively.
