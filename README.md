**Airbnb Price Prediction — Berlin** 
by Benjamin Caron

This project aims to predict the nightly price of Airbnb listings in Berlin using simple listing data (location, accommodation type, listing activity, etc).

**Objective**

Build a Machine Learning model capable of predicting the price of an Airbnb listing using variables such as:

- latitude / longitude

- neighbourhood_group

- room_type

- minimum_nights

- number_of_reviews

- reviews_per_month

- availability_365

- calculated_host_listings_count

**Data Preparation**

The dataset was cleaned and preprocessed using the following steps:

- removal of the text column neighbourhood

- filling missing values in reviews_per_month

- encoding categorical variables (neighbourhood_group, room_type)

- filtering prices within the range [20 €, 99th percentile]

**Trained Models**

- Baseline — Linear Regression

MAE = 48.17 €

RMSE = 69.31 €

- Main Model — Random Forest

MAE = 39.84 €

RMSE = 59.90 €

The Random Forest model significantly improves the baseline performance.

**Custom Prediction**

The notebook includes a function allowing the prediction of the price of a manually defined Airbnb listing.

Example:

Predicted price: 186.72 € / night

**Possible Improvements**

- filtering the number of nights sold per year

- adding new features (distance to city center, sunlight exposure, cleanliness rating)

- hyperparameter tuning of the Random Forest model

**Technologies**

- Python

- Pandas / NumPy

- scikit-learn

- Matplotlib / Seaborn
