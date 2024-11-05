# Ride Cost Analysis for Uber and Lyft

## Objective
The purpose of this project is to analyze the impact of weather conditions, location, and time on ride pricing for Uber and Lyft. The aim is to provide users insights on how to save money while using ride-sharing services in varying weather conditions.

## Background
Ride-sharing services like Uber and Lyft are popular for their convenience, but their dynamic pricing methods depend on multiple factors, including:

- **Time**: Prices often surge during peak hours or adverse weather, leading to significant cost differences for customers.
- **Location**: Pricing structures vary across different areas.
- **Weather**: Weather conditions impact passenger safety and can influence pricing.

Understanding these factors can help users make cost-effective choices and improve their overall ride-sharing experience.

## Data Source
The data for this project was obtained from Kaggle:
- **Dataset**: [Uber and Lyft Cab Prices Dataset](https://www.kaggle.com/datasets/ravi72munde/uber-lyft-cab-prices)

## Data Cleaning
The dataset was cleaned and preprocessed through the following steps:

1. **Missing Values**: Removed null rows in the cab ride dataset.
2. **Filled Null Entries**: Replaced missing values in the weather dataset's 'rain' column with zeros.
3. **Removed Duplicates**: Eliminated duplicate rows to avoid redundancy.
4. **Standardized Column Names**: Converted text to lowercase and removed extra spaces for consistency.
5. **Categorical Encoding**: Converted product IDs to user-friendly labels (e.g., 'Uber Taxi').
6. **Dropped Irrelevant Columns**: Removed columns like user ID that were not relevant to the analysis.
7. **Merged Datasets**: Combined cab and weather datasets based on relevant columns for a unified analysis.

## Exploratory Data Analysis (EDA)
Exploratory Data Analysis was conducted to visualize data distributions and relationships:

- **Distribution Analysis**: Examined prices across different cab types.
- **Correlation Heatmap**: Displayed relationships between features.
- **Scatter Plots**: Showed the relationship between price and distance.

Key findings highlighted price variations based on ride count, cab type requests, and feature correlations.

## Modeling Approaches
Multiple regression models were applied to predict ride prices:

1. **Linear Regression**
   - Accuracy: 76.93%
   - Provides a simple baseline model to understand feature influence.

2. **K-Nearest Neighbors (KNN)**
   - Accuracy: 76.15%
   - Captures complex relationships in the data.

3. **Random Forest**
   - Accuracy: 79.39%
   - Robust against overfitting, effectively handles complex data.

4. **Gradient Boosting**
   - Accuracy: 77.90%
   - Sequential tree-building improves predictive accuracy.

5. **Decision Tree**
   - Accuracy: 77.91%
   - Easy to interpret, captures non-linear interactions.

6. **Bagging Regressor**
   - Accuracy: 79.32%
   - Reduces variance by averaging multiple model predictions.

## Conclusion
This project provides valuable insights into how various factors affect Uber and Lyft ride costs, enabling users to make informed choices based on time, location, and weather conditions. Future work could focus on price prediction for different time frames or analyze price surges during specific hours.


## License
MIT License

Copyright (c) [2024] [Siri Duggineni]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
