# meme_stock_prices
Presentation: [Google Slides](https://docs.google.com/presentation/d/e/2PACX-1vRn1nLammvhjtL82N-8cUi9kMMcEskN5oxjqiU6lPaGUr0OKvJq94ZxSkmMC6jOHQNZ5nLYIMFumxyG/pub?start=true&loop=true&delayms=3000)
## Git Hub Branches and Communication 
Team members:
   * Guadalupe Salinas: [branch](https://github.com/gsalinas01/meme_stock_prices/tree/twitter_practice_api_pull)
   * Ricardo Saldana: [branch](https://github.com/gsalinas01/meme_stock_prices/tree/Ricky_Stock_Hist_query)
   * JT Carter: [branch](https://github.com/gsalinas01/meme_stock_prices/tree/Linear_Regression_Practice)
   * Stone Leiker: [branch](https://github.com/gsalinas01/meme_stock_prices/tree/Stone_Memestock)

## Background
Meme stocks have been gaining popularity in the last two years and have generated investors both profits and losses. The rise of social media fandom and its accompanying chatter has been named the culprit of major catapults in stocks such as GME, TSLA, AMC, and many others. 

## Overview
In this project we will test whether we can predict if the price of a meme stock will increase or decrease based on the social media hype around it, that is the conversations invoving their mention online. Specifically, we will be analyzing Twitter data to measure how often Tesla stock is mentioned in a 7 day period, and merging this data with the stock price counterpart on an hourly basis. 
As a baseline we will see if we can create the same results using a Stock index, such as the S&P500 index,  in lieu of the Twitter data. 

## Source data 
1. Historical Stock Data: 
For the stock data we used the Yfiance API python library.  With this python API library we were able to extract historical stock data, however we encountered the following limitation:  hourly data was limited to the previous 7 days.  
    1.  Data Acquire (Hourly Stock Data): % Stock Price change, Volume of stock exchanges for SP500 and TSLA stocks. 

2. Twitter - TSLA stock mention:
For twitter TSLA data we used the Twarc API python library.  This library uses the Twitter API to collect data.  The Twitter API also limited us to hourly data, for the previous 7 days. 
    1. Data Acquire (Hourly Tweet Count Data): Tweets that mentioned “#TSLA”, the common way to mention a stock ticker.
      * This analysis includes tweet data from the past 7 days at the start of the project. 
      * Data was extracted from twitter API, placed into a jupyter notebook dataframe, and cleaned up to include the date, hour, and tweet counts for the respective time frame. 
      * 

## Questions To Answer 
1.  Will a logistical regression model show that the quantity of Tweets mentioning #TSLA affect the price of Tesla stock? 
2.  What has a bigger impact on the price of a meme stock such as TSLA? (Tweet mention count data vs. S&P500)

## Results 
1. Linear Regression (because a linear regression was performed, however unfitting it was for our overall story purposes)
  * The linear regression models were performed on the following parameters:
    * Tesla percent day changes vs Tesla tweet counts
      * Results: Explanation
      * 
    * Tesla percent day changes vs SPY percent day changes
      * Results: Explanation 
      * 
    * & an overall volume vs Tesla percent day changes
      * Results:
      *         
3. Logistical Regression (Supervised Machine Learning)
4. 

What has the strongest correlation to TSLA (meme stock) price, SP500 or tweet post count?
        1.  First, show a Logistical regression model, and realized that it has a low accuracy rating. (y= % change, x=TSLA volume, SPY volume, spy % change, tweeter count too (1 week data)

        2. **** (Tentative talk to richard)****Second, PCA NN model and show how it has a higher accuracy success.  And now you will get the eigen value/vectors for SPY and tweeter count to determien which one has the highest correlation. (y= figure it out % change,  x=TSLA volume, SPY volume, spy % change, tweeter count too (we will do it for one day, and predict if it went up or down for each hour)



