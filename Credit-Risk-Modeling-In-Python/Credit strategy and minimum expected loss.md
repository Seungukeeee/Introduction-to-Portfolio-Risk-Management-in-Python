# Credit strategy and minimum expected loss

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Credit strategy and minimum expected loss
</aside>

- To discover the bad rate, an impact of each acceptance rate we could calculate all the values manually, or we could calculate them automatically and create a table. This table is referred to as **the strategy table** because we can choose our acceptance rate based on our overall strategy for the loan portfolio.
- The way to calculate
    - We first set up objects to store the values.
    - we also have two empty lists to store the thresholds and bad rates.
    
    ![image.png](image%2057.png)
    
    - To create the table, use a for loop to perform all of the calculations automatically and store the results.
    
    ![image.png](image%2058.png)
    
    - once the for loop completes, we can create a data frame for the strategy table which contains the values from each of the lists we made before.
    
    ![image.png](image%2059.png)
    
    ![image.png](image%2060.png)
    
    ![image.png](image%2061.png)
    
    ![image.png](image%2062.png)
    
    ** here, I assume each default in our accepted loans is a loss of the average amount of all loans. this gives a rought estimate for the portfolio value at each acceptance rate. 
    
    ** there is a trade-off between acceptance and bad rate.
    
- Total expected loss
    - it represents how much we expect to lose on loan defaults given their probability of default.
    
    ![image.png](image%2063.png)
    
    ![image.png](image%2064.png)
    
    ** Probability of Default (PD): the pro
    
    ** EAD(Exposure at Default): it **estimates the total amount of money the bank is *exposed to losing* at the time of default** — **not the loss itself**.
    
    ** Loss Given Default (LGD): estimates the percentage of the EAD that the bank will actually lose, after recoveries like collateral or legal actions.
    
    ** in simpler terms, EAD says “What’s at stake?”, LGD says “How much of that will we actually lose after trying to recover?”