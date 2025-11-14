> AAPL Stock Closing Price Prediction (Machine Learning Project)
> This project, developed for our Data Mining course, applies and compares multiple regression models to predict the closing price of Apple (AAPL) stock based on historical trading data.
> Key Finding: A simple Linear Regression model significantly outperformed more complex models (like Random Forest and Gradient Boosting), achieving an R² score of 98.37% and demonstrating superior stability during extreme market volatility.
>  Dataset
>  * Source: Kaggle - Stock Market Dataset
>  * File Used: AAPL.csv
>  * Time Range: 1980 - 2020 (40 years of daily stock data) 
>  Methodology
> We followed a strict methodology to ensure accurate results and prevent common pitfalls like data leakage.
> 1. Data Cleaning
>  * The Date column was converted to the proper datetime format.
>  * The dataset was checked for any missing values (NaNs) and duplicate rows. (Note: The initial check found a few missing values which were handled, resulting in a clean dataset for modeling) .
> 2. Train/Test Split (Preventing Data Leakage)
> To prevent time-series data leakage and simulate a realistic forecasting scenario, we split the data chronologically:
>  * Training Set: 1980 - 2019 (All data before the year 2020)
>  * Testing Set: 2020 data only
> 3. Models Implemented
> We trained and evaluated 6 different regression models to compare their performance:
>  * Linear Regression
>  * Decision Tree
>  * Random Forest
>  * K-Nearest Neighbors (KNN)
>  * Extra Trees
>  * Gradient Boosting
>  Results & Analysis
> The results clearly showed the superiority of the simple Linear Regression model for this specific task.
> Model Performance Comparison
> | Model | R² Score | RMSE |
> |---|---|---|
> | Linear Regression | 0.9837 | 3.77 |
> | Decision Tree | 0.6218 | 18.14 |
> | Random Forest | 0.5789 | 19.15 |
> | Gradient Boosting | 0.6050 | 18.54 |
> | Extra Trees | 0.5955 | 18.77 |
> | KNN | 0.3139 | 24.44 |
> Metrics derived from the test set (2020 data).
> Conclusion
> Contrary to common assumptions, the complex models (like Random Forest) were not the best fit. The reason is that Apple's long-term stock price follows a strong linear trend, which the Linear Regression model captured perfectly and efficiently.
> Stress Test: COVID-19 Market Crash Analysis
> We specifically analyzed the models' performance during the March 2020 market crash.
>  * Recovery Speed: The Linear Regression model needed only 2 weeks to recover its predictive accuracy.
>  * Other Models: Tree-based models required 4-6 weeks to recover, while KNN failed to recover completely.
>  * Insight: This proves that Linear Regression was not only the most accurate but also the most stable and robust model, adapting quickly to sudden market shocks.
>  Technologies Used
>  * Language: Python
>  * Environment: Google Colab
>  * Libraries:
>    * Pandas (Data manipulation and cleaning)
>    * Scikit-learn (Modeling and metrics)
>    * NumPy (Numerical operations)
>    * Plotly Express (Interactive visualizations)
>    * KaggleHub (Data import)
>   
>    * Team Members :
>  * Maha Alrashidi
>  * Nuha Alshammari
>  * Fajer Alfozan
