# meme_stock_prices

### Internal for Team use only
1. (Ricky)Create df for stock % daily change for 1 year: 
    1. TSLA 
    2. SPY Index (this will be our base) (Will come in handy if we do Neural Network (NN))
    
2. (Lupe)Create df for tweeter Eleon Musk total tweeter feed for 1 year: 
    1. (Better) total tweeks mentioning TSLA per day for last weak (all Tweets)
    
3. (Ricky)Create a combine df, columns as follows: 
    1. TSLA: % daily change, and close price
    2. SPY: % daily change, and close price
    3. Total Tweets qty per day
    
4. (JT )Linear Regression model
    1. Linear Reggression model: TSLA vs Spy 
        1. 2 graphs, show R value and P value for each
    2. PCA model:
        1. using combined DF (Section 3)
        2. y will be TSLA % change, x will be everything else
        3. See "Bonus" Neural Network idea #1

5. (Lupe/Ricardo/Stone) Build database
    1. IDK should we do postgre or do SQL/SQL lite ?

6. (Ricky/Stone)Build our website with the interative graphs


Bonus Neural Network idea #1
1. Create a predictive model to predict TSLA % change per day depending all 3 variables (SPY, Elons Tweets, Total TSLA Tweets) to figure out which one has the highest correlation (this will be used using the eigen values/vector method aka PCA) 


Presentation Rubric 
Overall Story: 



Team members have drafted their 
project, including the following: 
✓ Selected topic:
    1.  Are meme stock prices affected by tweet count? Specifically TSLA

✓ Reason why they selected their topic:
    1.  Meme stock popularity has risen within the last 2 years.  Our project wants to figure out if tweet chatter correlate to price % change of this stocks or are these stocks simply correlate to the S&P500 index, like the majority of all other stocks.

✓ Description of their source of data:
    1. Historical Stock Data: 
        1. For Historical stock data we used two(2) methods:  A freee yahoo API web Url and using yfiance python library.  Both methods used the same yahoo API, and the API had data limits as follows:  limits of hourly data was limited to 7 days, while daily historical data was limited to 5 years. 

    2. Tweet Chatter count Data:
        1.  For historical tweeter count data this project used Twarc python library.  This library uses tweeter API to collect data.  The limits of the tweeter api limited us to hourly data, for up to 7 days of tweeter count data for a specific query. 


✓ Questions they hope to answer with 
the data:
    1.  What has the strongest correlation to TSLA (meme stock) price, SP500 or tweet post count?
        1.  First we will show linear regression models for the year, but also explain that this type of model is limited since this is just long term trend. (TSLA and SPY, 1 year data)

        2. Second, Show a Logistical regression model, and realized that it has a low accuracy rating. ((TSLA and SPY (tweeter count too?), 1 year data))

        3. Third, PCA NN model and show how it has a higher accuracy success.  And now you will get the eigen value/vectors for SPY and tweeter count to determien which one has the highest correlation. (TSLA, SPY, tweeter count, 5 day data hourly)
        

Note: The content does not yet need to 
be in the form of a presentation; text in 

