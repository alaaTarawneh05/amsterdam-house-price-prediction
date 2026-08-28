# Amsterdam House Price Prediction

A machine learning project that analyzes housing data from Amsterdam and predicts house prices using Linear Regression. The project covers the complete workflow from data exploration and cleaning to outlier removal, feature analysis, model training, and performance evaluation.

## Project Overview

The objective of this project is to predict the price of residential properties in Amsterdam based on their physical and geographical characteristics.

The dataset is analyzed to identify relationships between house prices and features such as:

- Area
- Number of Rooms
- Longitude
- Latitude

Text-based address information and high-cardinality ZIP code values were excluded from the prediction model because they require additional preprocessing before being effectively used in a Linear Regression model.

## Data Preprocessing

The preprocessing workflow includes:

- Dataset structure and data type inspection
- Missing value detection and handling
- Duplicate record checking
- Removal of unnecessary index columns
- Exploratory analysis of address and ZIP code distributions
- Outlier detection using boxplots
- Outlier removal using the Interquartile Range (IQR) method

## Exploratory Data Analysis

The project performs statistical and visual analysis to better understand the dataset, including:

- Summary statistics
- Price range analysis
- Boxplots for numerical features
- Correlation analysis using a heatmap

The numerical features analyzed include:

- Price
- Area
- Room
- Longitude
- Latitude

## Machine Learning Model

A Linear Regression model is developed to predict property prices.

The workflow includes:

- Selecting Area, Room, Longitude, and Latitude as input features
- Using Price as the target variable
- Splitting the dataset into training and testing sets using an 80/20 split
- Standardizing numerical features using StandardScaler
- Training a Linear Regression model
- Generating predictions on unseen test data

## Model Evaluation

The model is evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- Error Ratio

The model achieved an R² score of approximately 0.536, explaining around 53.6% of the variation in Amsterdam house prices. The prediction error was also compared with the overall price range to provide additional context for evaluating model performance.

## Visualization

The final model performance is visualized using an Actual vs. Predicted Price scatter plot, allowing direct comparison between predicted house prices and their true values.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Key Concepts

- Exploratory Data Analysis
- Data Cleaning
- Missing Value Handling
- Duplicate Detection
- Outlier Detection
- IQR Method
- Correlation Analysis
- Feature Selection
- Feature Scaling
- Linear Regression
- Train-Test Split
- Regression Model Evaluation
