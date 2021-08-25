# GSTA: Gated Spatial-Temporal Attention Approach for Travel Time Prediction

A deep learning approach that uses a Gated Residual Network (GRN) and Gate Linear Unit (GLU) with Multi-Head attention and Feature Selection Module (FS) to predict travel times.

A sample of 81K trips is provided for each of the NYC and Chengdu Taxi datasets in folders (NYC Data, Chengdu Data).

The data samples are already pre-processed (Data Cleaning, Feature Engineering,... etc) and randomly split into train (X_train, Y_train), validation (X_val, Y_val), and test (X_test, Y_test).

The implementation of the prediction model for each dataset is given in a separate jupyter notebook (GSTA on NYC.ipynb, and GSTA on Chengdu.ipynb).

# Parameters:
1- optimizer=Adam(lr=0.001).
2- loss='mean_absolute_error'
3- metrics=['mae','mape']
4- Dropout=0.2
5- epochs = 50
6- batch_size = 256
7- kernel_regularizer=l2(0.001)
8- Activation('elu')
9- BatchNormalization(epsilon=1e-06, momentum=0.98)
10- kernel_initializer="he_uniform"

The dependent needed libraries are:

Keras 2.4.3, Tensorflow 2.3.0, Bokeh 2.2.1, Numpy 1.19.3, Pandas 1.1.5, Sklearn.

# Each sample is a json string. The key contains:


