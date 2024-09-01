# Housing Price Prediction

This project involves predicting housing prices using machine learning models. The dataset contains various features related to houses, and the goal is to predict the price of each house.

## Dataset

The dataset includes the following columns:
- `price`: The target variable we aim to predict.
- `area`: The area of the house.
- `bedrooms`: The number of bedrooms.
- `bathrooms`: The number of bathrooms.
- `stories`: The number of stories.
- `mainroad`: Indicates whether the house is on the main road.
- `guestroom`: Indicates the presence of a guestroom.
- `basement`: Indicates the presence of a basement.
- `hotwaterheating`: Indicates the presence of hot water heating.
- `airconditioning`: Indicates the presence of air conditioning.
- `parking`: The number of parking spaces.
- `prefarea`: Indicates whether the house is in a preferred area.
- `furnishingstatus`: The furnishing status of the house.

## Project Steps

1. **Data Preparation**
   - Loaded the dataset and handled missing values:
     - Filled missing values in numerical columns with the median.
     - Filled missing values in categorical columns with the mode (most frequent value).
   - Converted categorical features to numerical values using one-hot encoding.
   - Dropped unnecessary columns such as `Id` and `price` from the feature set.

2. **Model Training and Evaluation**
   - Split the data into training and testing sets.
   - Trained the following models:
     - Linear Regression
     - Random Forest Regressor
     - Support Vector Regressor (SVR)
     - Voting Regressor (combining Linear Regression, Random Forest, and SVR)
   - Evaluated the models using Mean Squared Error (MSE) and R-squared (R2) score.

3. **Results Visualization**
   - Compared the performance of the models by plotting True Prices vs. Predicted Prices for each model.

## Code

The code for data preparation, model training, evaluation, and visualization is provided in the script.

### Dependencies

The following Python libraries are required:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

You can install the required libraries using pip:
```bash
pip install pandas numpy matplotlib scikit-learn

