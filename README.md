# House Price Prediction in the USA

This project aims to predict the price of a house based on various features such as the number of bedrooms, bathrooms, living area size, and more. The prediction model is built using the `LinearRegression` model from the `scikit-learn` library.

## Dataset
The dataset contains various features that describe the characteristics of houses in the USA. These features help in predicting the price of the house.

### Key Features:
- **Date**: Date of recording the data for the house
- **No. of Bedrooms**: Total number of bedrooms
- **No. of Bathrooms**: Total number of bathrooms
- **Living Area**: Living area in square feet
- **Lot Area**: Lot area in square feet
- **Floors**: Number of floors in the house
- **Waterfront**: Whether the house has a waterfront view
- **View**: View rating of the house
- **Condition**: Overall condition of the house
- **Above Area**: Square feet of the house above ground level
- **Basement Area**: Square feet of the house's basement
- **Year Built**: Year the house was built
- **Year Renovated**: Year the house was last renovated
- **Street**: Street where the house is located
- **City**: City where the house is located
- **StateZip**: State and ZIP code of the house
- **Country**: Country of the house

The **output** is the **price** of the house.

## Libraries Required
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

To install the necessary libraries, run:
```bash
pip install pandas numpy matplotlib scikit-learn
```

## Preprocessing of the Data
1. **Date Removal**: The `date` column is removed as it is not relevant for price prediction.
2. **Encoding**: All categorical columns are encoded using the `OneHotEncoder` from the `scikit-learn` library.
3. **Scaling**: All numeric columns are scaled using the `MinMaxScaler` to bring them to a uniform scale.

## Model Training
- **Algorithm**: The model uses `LinearRegression` from `scikit-learn`.
- **Train-Test Split**: The dataset is split into 80% training data and 20% testing data using the `train_test_split` function from `scikit-learn`.
- **Evaluation**: The trained model is evaluated on the following metrics:
  - **Mean Absolute Error (MAE)**
  - **Mean Squared Error (MSE)**
  - **Root Mean Squared Error (RMSE)**

## How to Run the Project
1. Clone the repository:
    ```bash
    git clone <repository-link>
    ```
2. Download the dataset and preprocess it as per the instructions.
3. Run the training script or Jupyter Notebook to train the model on the preprocessed dataset.

## Features
- **Machine Learning Model**: The project uses `LinearRegression` which performs continuous linear regression.
- **Evaluation**: After training, the model is evaluated using various metrics like MAE, MSE, and RMSE to assess performance.

## Future Improvements
- Explore other regression models like Decision Trees, Random Forest, or Gradient Boosting for better accuracy.
- Add more features to improve the prediction accuracy.

---
