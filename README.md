# Stock prediction - Facebook-Prophet
This project is to build an stock price predictor for any stock just by typing its Ticker symbol.

## Loading the data  
Loaded the stock price data from yfinance by Yahoo Finance.
## Stock data for 1 year

![Screenshot (43)](https://user-images.githubusercontent.com/78019202/179429562-44cc5e57-e97e-4295-b40e-129da0677895.png)


## Data Visulatization  
Data Visulatization with Plotly Express.  
## Plotly Area Close Price
![Screenshot (58)](https://user-images.githubusercontent.com/78019202/179430647-5429849c-5d77-45f8-a1c0-bd475a16bbdc.png)

## Plotly Line Close Price


![Screenshot (51)](https://user-images.githubusercontent.com/78019202/179429824-f5188c04-89da-4113-be48-849454babbfa.png)
## Plotly Area Volume

![Screenshot (52)](https://user-images.githubusercontent.com/78019202/179429950-534b99d5-c52d-4bf2-8ff6-7735eb8620bf.png)

## Plotly Bar Volume
![Screenshot (53)](https://user-images.githubusercontent.com/78019202/179430066-184579eb-0bab-4a15-bb3f-53f6e0880509.png)
## Plotly Box Close Price
![Screenshot (54)](https://user-images.githubusercontent.com/78019202/179430142-1d08b497-c763-4d1a-84cd-38d0529ec2be.png)
## Facebook Prophet
**Accurate and Fast:** It is accurate and generate results very fast.  
**Reliable:** Facebook Company itself uses Prophet for Internal forecasting.  
**Fully Automatic:** Works with missing data and no need to perform extensive data processing.  
**Domain Knowledge Integration :** Forecasting can be made better by adding domain knowledge expertise like holidays and patterns.  
**Available in R and Python:** We will be using python programming Language.

## Data Preparation

Convert "Date" and "Close" data to "ds" and "y".

![Screenshot (59)](https://user-images.githubusercontent.com/78019202/179430520-14f9859f-995e-4a12-a9a0-71160da8a669.png)

## Facebook Prophet Model
Build the model with-  
*m=Prophet()  
m.fit(prophet_df)*

## Forecasting 
*future = m.make_future_dataframe(periods=30)  
forecast=m.predict(future)*


## Forecated vs Original price along with 30 days future price
![forecasted vs original along with future 30 days price](https://user-images.githubusercontent.com/78019202/179429366-c7df9d83-a02b-420c-9604-e1e265d46554.png)

## Components of Forecast

![components of forecast](https://user-images.githubusercontent.com/78019202/179429439-cce85970-eb1a-4412-b6c9-324a8e55f50b.png)

## Future 30 Days price
![Screenshot (60)](https://user-images.githubusercontent.com/78019202/179430427-057989d5-818f-474f-b55b-35b62168e367.png)
## Downloading Forecasted Data

Download the data forecasted data with the following code-

*from google.colab import files*      
*forecast.to_csv(stock + '_forecast.csv')*  
*files.download(stock+'_forecast.csv')*
