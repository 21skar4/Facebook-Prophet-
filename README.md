# Stock prediction - Facebook-Prophet
This project is to build an stock price predictor for any stock just by typing its Ticker symbol.

## Loading the data  
Loaded the stock price data from yfinance by Yahoo Finance.
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## Data Visulatization  
Data Visulatization with Plotly Express.  
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
  
## Facebook Prophet
**Accurate and Fast:** It is accurate and generate results very fast.  
**Reliable:** Facebook Company itself uses Prophet for Internal forecasting.  
**Fully Automatic:** Works with missing data and no need to perform extensive data processing.  
**Domain Knowledge Integration :** Forecasting can be made better by adding domain knowledge expertise like holidays and patterns.  
**Available in R and Python:** We will be using python programming Language.

## Data Preparation

Convert "Date" and "Close" data to "ds" and "y".
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

## Facebook Prophet Model
Build the model with-  
*m=Prophet()  
m.fit(prophet_df)*

## Forecasting 
*future = m.make_future_dataframe(periods=30)  
forecast=m.predict(future)*

## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Forecated vs Original price along with 30 days future price

![App Screenshot](forecasted vs original along with future 30 days price.png)
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
## Downloading Forecasted Data

Download the data forecasted data with the following code-

*from google.colab import files*      
*forecast.to_csv(stock + '_forecast.csv')*  
*files.download(stock+'_forecast.csv')*
