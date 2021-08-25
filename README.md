# GSTA: Gated Spatial-Temporal Attention Approach for Travel Time Prediction
- A deep learning approach that uses a Gated Residual Network (GRN) and Gate Linear Unit (GLU) with Multi-Head attention and Feature Selection Module (FS) to predict travel times. -A sample of 81K trips is provided for each of the NYC and Chengdu Taxi datasets in folders (NYC Data, Chengdu Data). 
- The data samples are already pre-processed (Data Cleaning, Feature Engineering,... etc) and randomly split into train (X_train, Y_train), validation (X_val, Y_val), and test (X_test, Y_test). 
- The implementation of the prediction model for each dataset is given in a separate jupyter notebook (GSTA on NYC.ipynb, and GSTA on Chengdu.ipynb).

# Parameters:
(These parameteres are tuned with whole dataset, you can change them manually)<br />
The default parameters are: <br />
1- optimizer=Adam(lr=0.001).  <br />
2- loss='mean_absolute_error' <br />
3- metrics=['mae','mape'] <br />
4- Dropout=0.2 <br />
5- epochs = 50 <br />
6- batch_size = 256 <br />
7- kernel_regularizer=l2(0.001) <br />
8- Activation('elu') <br />
9- BatchNormalization(epsilon=1e-06, momentum=0.98) <br />
10- kernel_initializer="he_uniform" <br />
11- num_heads = 4  , which is the number of heads in Multi-Head attention. 

# Best Model
The best model for each data during training phase is saved to folder "Models" as hdf5 file.

# Data sample
Each data sample is a CSV file. The key contains: <br />
* 


# Dependent libraries:
Keras 2.4.3, Tensorflow 2.3.0, Bokeh 2.2.1, Numpy 1.19.3, Pandas 1.1.5, Sklearn.



