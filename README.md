Data Mining Project: Apple (AAPL) Stock Price Prediction
This project, submitted for the "Data Mining" course at [University of Hail], focuses on building and comparing various machine learning models to predict the closing price of Apple (AAPL) stock.
Project Objective
The primary objective is to answer the question: "Which model most accurately predicts stock prices based on historical data?"
This is achieved by:
 * Implementing 6 different machine learning models.
 * Comparing their performance using precise metrics (R² and RMSE).
 * Testing the "robustness" of the models by analyzing their performance during extreme market volatility (e.g., the COVID-19 crash in March 2020).
Methodology
 * Data Source: Historical Apple (AAPL) stock data from 1980 to 2020, sourced from Kaggle.
 * Data Cleaning: Preprocessing involved handling missing values and removing duplicate entries.
 * Data Splitting:
   * Training Period: 1980 - 2019
   * Testing Period: 2020 data only
 * Features & Target:
   * Features: Open, High, Low, Volume
   * Target: Close (predicting the closing price)
Model Performance Comparison (Results)
Six models were evaluated. The performance results on the 2020 test dataset are as follows:
| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | 0.983 | 3.76 |
| Gradient Boosting | 0.605 | 18.54 |
| Extra Trees | 0.595 | 18.76 |
| Decision Tree | 0.621 | 18.14 |
| Random Forest | 0.578 | 19.14 |
| KNN | 0.313 | 24.44 |
*Results sourced from the project's final presentation.
Main Findings
The Linear Regression model significantly outperformed all other models.
 * Reasoning: Apple's stock price exhibits a very strong, long-term linear trend. The Linear Regression model, by its nature, is best suited to capture and extrapolate this dominant pattern.
 * More complex, non-linear models (like Decision Trees and Random Forest) performed poorly, likely due to overfitting or attempting to find intricate patterns that were not as significant as the primary trend.
 Crisis Performance Analysis (COVID-19 Stress Test)
When analyzing performance during the March 2020 market crash:
 * Linear Regression: Was the fastest to recover (took only two weeks to regain its accuracy).
 * Tree-based Models: Took 4-6 weeks to recover.
 * KNN: Failed to recover fully.
Tools & Libraries Used
 * Python
 * Pandas (for data processing and manipulation)
 * Scikit-learn (for model building, training, and metrics)
 * Plotly Express (for data visualization)
 * KaggleHub (for data retrieval)
 * Team Members: 
1- Maha Alrashid
2- Nuha Alshammari
3- Fajer Alfozan
