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

