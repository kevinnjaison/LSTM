# AirPassengers LSTM Prediction

This project demonstrates the use of a Long Short-Term Memory (LSTM) neural network to predict the number of monthly international air passengers based on historical data.

## Project Structure

## Requirements

The following Python libraries are required to run the notebook:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `tensorflow`

You can install the required libraries using the following command:

```bash
pip install pandas numpy matplotlib scikit-learn tensorflow

Data Loading and Preprocessing:

The dataset is loaded using pandas.
The Month column is converted to a datetime format and set as the index.
The data is scaled to a range of 0 to 1 using MinMaxScaler.
Sequence Creation:

Sequences of 12 months are created to predict the next month's passenger count.
Train-Test Split:

The data is split into training (80%) and testing (20%) sets.
Model Building:

An LSTM model is built using TensorFlow's Keras API.
The model consists of one LSTM layer and one Dense layer.
Model Training:

The model is trained for 50 epochs with a batch size of 16.
Prediction and Visualization:

Predictions are made on the test set.
The scaled predictions are reversed to their original range.
A plot is generated comparing the actual and predicted passenger counts.
