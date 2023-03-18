# Earthquake Prediction for Last 30 Days using Simple MLP and Rolling Window
This project predicts earthquakes around the world for the last 30 days using earthquake data obtained from the United States Geological Survey (USGS). We are using a simple Multilayer Perceptron (MLP) neural network and the rolling window concept to predict the earthquakes.

### Dataset
The dataset used is provided by the USGS and can be accessed through their Earthquake Catalog Search. The dataset contains information about earthquakes around the world, including the location, magnitude, depth, and time of occurrence.

### Model
The model used for this project is a simple MLP neural network that predicts the magnitude of an earthquake based on its location, depth, and time of occurrence. We are using the rolling window concept to feed the network with time-series data in order to predict future earthquakes.

### Rolling Window
We are using a rolling window of size window_size to prepare the input data for the network. The rolling window slides over the time-series data and selects window_size consecutive data points as the input for the network. This process is repeated for every time-step in the time-series data.

### Training
The model was trained using the last 30 days of earthquake data from the USGS. The data was preprocessed using the rolling window concept and split into a training set and a validation set. The model was trained using the training set and evaluated using the validation set.
