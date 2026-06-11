# Medical Insurance Cost Prediction using ANN

## Dataset

Medical Insurance Cost Dataset

Records: 1338

Target Variable:

* charges

Features:

* age
* sex
* bmi
* children
* smoker
* region

## Preprocessing

* Checked missing values
* No missing values found
* Applied One-Hot Encoding on:

  * sex
  * smoker
  * region
* Applied Standard Scaling on numerical features

## ANN Architecture

Input Layer

Dense(64, ReLU)

Dropout(0.2)

Dense(32, ReLU)

Dense(16, ReLU)

Output Layer Dense(1, Linear)

## Training Configuration

Optimizer:

* Adam

Loss Function:

* Mean Squared Error (MSE)

Metrics:

* Mean Absolute Error (MAE)

Early Stopping:

* Patience = 10

Batch Size:

* 32

Epochs:

* 100

## Evaluation Metrics

* MAE
* MSE
* RMSE
* R² Score

## Results

Higher R² and lower MAE/RMSE indicate better model performance.

## Future Improvements

* Hyperparameter tuning
* Batch Normalization
* More hidden layers
* Cross Validation
* Feature Engineering

## Troubleshooting

TensorFlow Not Found:

pip install tensorflow

Scikit-Learn Not Found:

pip install scikit-learn

Matplotlib Not Found:

pip install matplotlib

Shape Mismatch Errors:

Ensure the same preprocessing pipeline is applied to both training and testing data.
