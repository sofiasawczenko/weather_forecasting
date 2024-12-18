# Weather Forecasting for New York City

This repository contains a weather forecasting project for New York City using machine learning techniques, specifically Linear Regression and Ridge Regression. The goal is to predict weather conditions based on historical data from 1970 to 2022.

## Project Stages

### 1. Data Collection  
The historical weather data for New York City from 1970 to 2022 was collected from reliable sources. The dataset includes various features such as:

- Maximum Temperature
- Minimum Temperature
- Humidity
- Wind Speed
- Precipitation

### 2. Data Cleaning  
Before proceeding with the analysis, the data underwent a rigorous cleaning process to ensure its quality. The steps included:

- Removing missing values
- Correcting outliers
- Normalizing data  

This process made the dataset ready for training the machine learning models.

### 3. Data Preparation for Machine Learning  
The data was split into two subsets:

- **Training Set**: Used to train the models.
- **Testing Set**: Used to evaluate the models after training.

Additionally, relevant features were selected and transformed into a suitable format for feeding the regression models. **Normalization** was applied to ensure that all features had comparable scales, which is important for the regression models to perform accurately.

### 4. Model Training  
Two regression models were employed in this project:

- **Linear Regression**
- **Ridge Regression**

The models were implemented using the **scikit-learn (sklearn)** library. The training set was used to teach the models the patterns within the historical data.

### 5. Model Evaluation  
The models were evaluated using the testing set. The performance of the models was measured using the following metrics:

- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**

By comparing these metrics for both models, we were able to determine which model provided more accurate weather predictions.

## Technologies Used

- **Python**: The main programming language used for the implementation.
- **Pandas**: Used for data manipulation and analysis.
- **Scikit-learn (sklearn)**: Used to build and train the regression models.
- **Jupyter Notebook**: Used for interactive coding and data analysis.

## Requirements

To run this project, you will need the following Python packages:

- pandas
- scikit-learn
- matplotlib
- jupyter

**You can install the required packages using the following:**

```bash
pip install pandas scikit-learn matplotlib jupyter
```

## Conclusion

### Model Accuracy:
- The Mean Absolute Error (MAE) for the model is approximately 5.14 (initial evaluation) and 4.79 (after incorporating rolling and averaging features). This indicates the average difference between the predicted and actual temperatures is about 5.14°F and 4.79°F, respectively.
- Mean Squared Error (MSE) for the refined model is approximately 37.62, which quantifies the average squared difference between actual and predicted temperatures.

### Prediction Quality:
- The largest prediction errors occur on specific dates, with some of the highest discrepancies recorded on March 26, 2007, where the model predicted 49.74°F compared to the actual temperature of 78°F, resulting in a 28.26°F error.
- Other significant prediction errors were observed on January 2, 1999, March 26, 1998, and April 18, 1985, where errors in predictions were in the range of 26-30°F.

### Feature Importance:
- From the model's coefficients, it is evident that `tmax` (maximum temperature) and `tmin` (minimum temperature) are the most influential predictors in the model, with `tmax` having a coefficient of 0.447 and `tmin` with 0.517.
- The precipitation (`prcp`) and snow depth (`snow`, `snwd`) also influence the predictions, but their impact is lower compared to the temperature variables.

### Improvement Through Features:
- The model's performance improved after adding rolling averages for temperature and precipitation over different horizons (3-day, 14-day).
- Additionally, monthly and daily averages for temperature and precipitation significantly contributed to enhancing the model's ability to predict more accurately.

### Overall Insights:
- The model provides reasonable forecasts with an MAE below 5°F, and the accuracy improves when adding smoothing features like rolling and moving averages.
- Specific weather anomalies (such as abrupt changes in temperature) still pose challenges for the model, but overall, it performs well for general forecasting with a focus on the maximum temperature as the key predictor.

