# GSTA: Gated Spatial-Temporal Attention Approach for Travel Time Prediction

A deep learning approach to predict travel times.

This code is an implemnetaion of the paper titled "GSTA: Gated Spatial-Temporal Attention Approach for Travel Time Prediction".

A sample of 81K trips is provided for each of the NYC and Chengdu Taxi datasets in folders (NYC Data, Chengdu Data).

The data samples are already pre-processed (Data Cleaning, Feature Engineering, ...etc) and randomly splitted into train (X_train, Y_train), validation (X_val, Y_val), and test (X_test, Y_test).

The implementation of the prediction model for each dataset is given in a separate jupyter notebook (GSTA on NYC.ipynb, and GSTA on Chengdu.ipynb).

The dependent needed libraries are:

Keras 2.4.3

Tensorflow 2.3.0

Bokeh 2.2.1

Numpy 1.19.3

Pandas 1.1.5

Sklearn


