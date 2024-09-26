# Stock Data Prediction

 
                           <img width="678" alt="image" src="https://github.com/user-attachments/assets/af9666d1-7e96-4bc7-a107-13ad185374ff">



## Overview

This project implements various financial analyses and stock market prediction techniques using historical stock data for well-known companies such as Microsoft (MSFT), JPMorgan (JPM), ExxonMobil (XOM), NextEra Energy (NEE), and Procter & Gamble (PG). The notebook performs data preprocessing, exploratory data analysis (EDA), moving average comparisons, risk and return calculations, Monte Carlo simulations, and portfolio optimization.

## Key Features:
##### Data Loading: Uses the yfinance API to fetch 10 years of historical stock data.
##### Exploratory Data Analysis (EDA): Includes missing value checks, descriptive statistics, and graphical analysis of stock prices and returns.
##### Portfolio Optimization: Calculation of optimal portfolio weights for minimizing risk using the covariance matrix of log returns.
##### Monte Carlo Simulation: Simulates future stock prices based on historical data using the Monte Carlo method.
##### Annual Return Triangle: Graphically represents annual returns over multiple timeframes.
##### Moving Averages: Comparison of 50-day, 100-day, and 200-day moving averages.


## Prerequisites

Before running the project, ensure you have the following installed:

Python 3.x
Jupyter Notebook
Necessary Python packages:
Copy code
pandas
numpy
scikit-learn
matplotlib
seaborn
plotly
cufflinks
yfinance
tqdm
Installation

## Clone the repository and install the required packages:

##### git clone https://github.com/your-username/stock-data-prediction.git

## Data Analysis

The project uses stock data from the following companies:

Microsoft (MSFT)
JPMorgan Chase (JPM)
ExxonMobil (XOM)
NextEra Energy (NEE)
Procter & Gamble (PG)
Exploratory Data Analysis (EDA)
EDA includes generating descriptive statistics, checking for missing values, and plotting the adjusted closing prices of stocks. The descriptive statistics summarize the central tendency and variability in the data.

## Example statistics for stock prices:

Stock	Mean Price	Standard Deviation	Min Price	Max Price
MSFT	132.91	96.85	26.14	359.49
JPM	88.92	35.53	38.06	162.89
Moving Averages Comparison
Comparison of moving averages for different windows (50, 100, and 200 days) helps identify long-term trends.

## Annual Risk and Return
A function is created to calculate the annual risk and return based on daily returns:

Stock	Annual Return	Annual Risk
MSFT	28.4%	27.3%
JPM	16.9%	27.0%
Annual Return Triangle
A return triangle is generated for each stock, visualizing the annualized returns for different time windows.

## Portfolio Optimization

Using historical data, we optimize the portfolio for minimal risk by calculating the covariance matrix and minimizing portfolio volatility.

## Optimal Weights for Minimum Volatility Portfolio:

[0.0654, 0.0549, 0.1864, 0.5386, 0.1545]
##### Portfolio Return: 10.93%
##### Portfolio Risk: 16.22%

                   <img width="740" alt="image" src="https://github.com/user-attachments/assets/5ea77171-6260-4cb6-aa85-37b94eda238a">


## Monte Carlo Simulation

Monte Carlo simulations predict future stock prices based on historical price movements. The simulations provide a range of possible outcomes, including the mean, max, min, and percentiles.

## Example for Microsoft (MSFT):

                     <img width="740" alt="image" src="https://github.com/user-attachments/assets/e0701000-2ecc-442e-8ef3-26a8a2b743f1"> 

Mean: 361.10
Max: 635.36
Min: 176.49
5th Percentile: 250.60
95th Percentile: 510.72
Usage

## Run the Jupyter notebook:

##### jupyter notebook Stock_Data_Prediction.ipynb

## Follow the steps in the notebook to preprocess the data, analyze stocks, run simulations, and optimize your portfolio.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to enhance the model accuracy or add new features.
