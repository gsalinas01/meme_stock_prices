# meme_stock_prices

## Git Hub Branches and Communication 
1. Team Members and Branches

## Background
Meme stocks have been gaining increasing popularity in the past two years and have generated investors both profits and losses. The rise of social media fandom and the sharing of memes about certain stocks creates online chatter than can in theory catapult stock up and vise versa. 

## Selected Topic
In this project we will try to answer the question, can we predict if a meme stock will go up or down based on the social media hype. Specifically, we will be analyzing Twitter data to measure how often Tesla stock is mentioned. 
As a baseline we will see if we can create the same results using a Stock index, such as the S&P500 index,  in lieu of the Twitter data. 

## Source data 
1. Historical Stock Data: 
For Historical stock data we used Yfiance API python library.  With this python API library we were able to extra historical stock data but the API had data limits as follows:  limits of hourly data was limited to the previous 7 days.  
    1.  Data Acquire (Hourly Stock Data): % Stock Price change, Volume of stock exchanges for SP500 and TSLA stocks. 

2. Tweet Chatter count Data:
For historical tweeter count data this project used the Twarc API python library.  This library uses twitter API to collect data.  The twitter api limited us to hourly data, for up to 7 days of tweeter count data for a specific query. 
    1. Data Acquire (Hourly Tweet Count Data): Tweets that mentioned “#TSLA”, the common way to mention a stock ticker. 

## Questions To Answer 
1.  Will a logistical regression model show that tweets count affect the price of TSLA. 
2.  What has a bigger impact on the price of a meme stock such as TSLA. 

## Results 
1. Logistical Regression (Supervised Machine Learning)
2. 

What has the strongest correlation to TSLA (meme stock) price, SP500 or tweet post count?
        1.  First, show a Logistical regression model, and realized that it has a low accuracy rating. (y= % change, x=TSLA volume, SPY volume, spy % change, tweeter count too (1 week data)

        2. **** (Tentative talk to richard)****Second, PCA NN model and show how it has a higher accuracy success.  And now you will get the eigen value/vectors for SPY and tweeter count to determien which one has the highest correlation. (y= figure it out % change,  x=TSLA volume, SPY volume, spy % change, tweeter count too (we will do it for one day, and predict if it went up or down for each hour)



