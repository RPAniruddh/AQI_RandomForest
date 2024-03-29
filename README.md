# Air Quality Index (AQI) Prediction using Random Forest 

This program aims to create a machine learning prediction model using the Random Forest algorithm to accurately forecast the Air Quality Index (AQI) for the next three days, specifically to compare its performance with LSTM and ARIMA models for the same. The model is trained using historical AQI data specific to Vyttila

## Dataset

The dataset used for training the model is named "vyttiladateupdate.csv". It contains the following fields:
- Place: Location of measurement
- Date: Date of measurement
- PM10: Particulate Matter (PM) with a diameter of 10 micrometers or less
- PM2.5: Particulate Matter (PM) with a diameter of 2.5 micrometers or less
- CO: Carbon Monoxide levels
- AQI: Air Quality Index

The dataset covers the period from August 2022 to December 2023, providing ample data for training and testing the model.

## Installation

To run the code, you need to have Python installed on your system along with the following dependencies:

- pandas
- scikit-learn
- numpy
- matplotlib

You can install these dependencies using pip:

```bash
pip install pandas scikit-learn numpy matplotlib
