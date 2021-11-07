# meme_stock_prices

### Internal for Team use only
1. (Ricky)Create df for stock % daily change for 1 year: 
    1. TSLA 
    2. SPY Index (this will be our base) (Will come in handy if we do Neural Network (NN))
    3. ***** wiat on this DF for top 50 from the last 2 year 
    
2. (Lupe)Create df for tweeter Eleon Musk total tweeter feed for 1 year: 
    1. (Better) total tweeks mentioning TSLA per day for last year (all Tweets)
    2. ***** (if We have time) will be to just do total tweeks per day for Elon Musk by day
        1. (Better) add a column for what Musk said in tweet (Will come in handy if we do Neural Network)
    
3. (Ricky)Create a combine df, columns as follows: 
    1. TSLA: % daily change, and close price
    2. SPY: % daily change, and close price
    3. Total Tweets qty per day
    4. **** Elon Musk qty of memes per day
    
4. (JT )Linear Regression model
    1. TSLA vs Spy (2 years)
    2. TSLA vs total tweeks mentioning TSLA (2 years)
    3. TSLA vs qty of Elon musk Tweeks
    4. Normal distrubution of # TSLA tweets per day??? (maybe)
    
5. (Ricky/Stone)Build our website with the interative graphs


Bonus Neural Network idea #1
1. Create a predictive model to predict TSLA % change per day depending all 3 variables (SPY, Elons Tweets, Total TSLA Tweets) to figure out which one has the highest correlation (this will be used using the eigen values/vector method aka PCA) 


Bonus Neural Network idea #2
1. Using Elon Musk tweet data to add columns to our combine DF: 
    1.  Using Natural language (Module 16): remove all filler words, and only use key words, use top 10 key words or bucket positive words
2. Encode the additional words into columns
3. Run a Neural Network (NN) model which words

