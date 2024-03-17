# Air Quality Index (AQI) Prediction using Random Forest

This program aims to create a machine learning prediction model using the Random Forest algorithm to accurately forecast the Air Quality Index (AQI) for the next three days. The model is trained using historical AQI data specific to Vyttila.

## Dataset

The dataset used for training the model is named "vyttiladateupdate.csv". It contains the following fields:
- Place: Location of measurement
- Date: Date of measurement
- PM10: Particulate Matter (PM) with a diameter of 10 micrometers or less
- PM2.5: Particulate Matter (PM) with a diameter of 2.5 micrometers or less
- CO: Carbon Monoxide levels
- AQI: Air Quality Index

The dataset covers the period from August 2022 to December 2023, providing ample data for training and testing the model.

## Getting Started

To run the program, follow these steps:

1. Clone this repository to your local machine.
2. Ensure you have Python installed along with the necessary libraries specified in `requirements.txt`.
3. Download the dataset file "vyttiladateupdate.csv" and place it in the appropriate directory.
4. Open the Jupyter Notebook file "RandomForest.ipynb" in your preferred environment.
5. Execute the code cells in the notebook to train the model and make predictions.

## Model Training

The Random Forest algorithm is used to train the prediction model. The following steps are performed during training:

1. Load the dataset and preprocess it, including converting the 'Date' field to datetime and extracting relevant features.
2. Split the dataset into training and testing sets.
3. Train the Random Forest model using the training data.
4. Evaluate the model's performance on the test data using Root Mean Squared Error (RMSE).

## Prediction and Inverse Normalization

Once the model is trained, it predicts the AQI values for the specified time frame. Inverse z-score normalization is then applied to obtain the actual AQI values. The inverse normalization process involves:

1. Calculating the mean and standard deviation of the original AQI values in the dataset.
2. Reverting the normalized predictions to their original scale using the mean and standard deviation.

## Results

The model's performance is assessed using RMSE on normalized predictions. Additionally, the first five reverted predictions are printed to demonstrate the model's forecasting capability.

## Note

Ensure that the dataset file path is correctly specified in the code before running the program.

For any issues or inquiries, please contact [maintainer_name](mailto:maintainer_email).

