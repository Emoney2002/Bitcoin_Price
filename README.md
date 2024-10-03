# Bitcoin_Price
Bitcoin Price Prediction Model
This project focuses on building a machine learning model to predict the closing price of Bitcoin using historical price data. I perform exploratory data analysis (EDA) on the dataset and develop a regression model (Linear Regression) to predict the closing price based on other factors such as the opening price, highest price, lowest price, trading volume, and market capitalization.

Table of Contents
Project Overview
Dataset
Exploratory Data Analysis (EDA)
Model
Performance
Requirements
Installation
Usage
Results
Conclusion
Future Work

Project Overview
The main objective of this project is to predict the closing price of Bitcoin based on historical price data and other financial indicators. We use data from a given training dataset, conduct extensive exploratory data analysis, and train a Linear Regression model. The performance of the model is then tested on a separate test dataset.

Dataset
I used two CSV files:

bitcoin_price_Training.csv: Training data with historical Bitcoin prices and related features.
bitcoin_price_Test.csv: Test data used to evaluate model performance.
Features:
Date: Date of the record.
Open: Opening price of Bitcoin on that day.
High: Highest price on that day.
Low: Lowest price on that day.
Close: Closing price on that day (target variable for prediction).
Volume: Total trading volume on that day.
Market Cap: Market capitalization of Bitcoin.
Exploratory Data Analysis (EDA)
The EDA step involved:

Cleaning the dataset by handling missing values and formatting columns.
Visualizing the historical trends in Bitcoin's price and trading volume.
Plotting the correlation matrix to analyze relationships between variables.
Identifying trends and seasonality in the time series data.
Key Insights:

There is a strong correlation between the Open, High, Low, and Close prices.
Trading volume has a moderate correlation with Bitcoin prices.
The Bitcoin price has shown significant fluctuations, with large spikes in the closing price over time.
Model
We used a Linear Regression model to predict the closing price. The input features for the model were:

Open price
High price
Low price
Volume
Market Cap
Training Process:
The dataset was split into training and validation sets.
The model was trained on the training set, and performance was evaluated on both validation and test datasets.
Performance
The model achieved the following performance on the test dataset:

Mean Squared Error (MSE): 3302
R² Score: 0.9503 (The model explains 95% of the variance in the closing price).
The predictions were generally accurate, although some differences between actual and predicted values were observed, especially for days with extreme market volatility.

Requirements
To run the project, you will need the following dependencies:

Python 3.x
pandas
numpy
scikit-learn
matplotlib
seaborn
Jupyter Notebook (optional, for running in an interactive environment)

Results
The Linear Regression model successfully predicted the closing prices of Bitcoin with an R² score of 0.9503 on the test dataset. The model accurately captured the overall trends in Bitcoin prices, but could be further optimized to reduce the mean squared error.

Sample predictions:

Date	Open	High	Low	Volume	Market Cap	Predicted Close
2017-08-07	3212.78	3397.68	3180.89	1,482,280,000	52,987,300,000	3324.22
2017-08-06	3257.61	3293.29	3155.60	1,105,030,000	53,720,900,000	3216.14
2017-08-05	2897.63	3290.01	2874.83	1,945,700,000	47,778,200,000	3143.93
Conclusion
The project demonstrated that a simple Linear Regression model can be effective in predicting Bitcoin prices based on historical data. However, there is room for improvement, particularly in reducing prediction error during high-volatility periods.

Future Work
To further improve the model, the following steps could be taken:

Experimenting with more complex models like Random Forests or Gradient Boosting.
Incorporating additional features such as sentiment analysis from news or social media.
Analyzing the impact of external factors like market regulations or major economic events on Bitcoin prices.
