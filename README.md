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

You can install the required packages using the following:

```bash
pip install pandas scikit-learn matplotlib jupyter
