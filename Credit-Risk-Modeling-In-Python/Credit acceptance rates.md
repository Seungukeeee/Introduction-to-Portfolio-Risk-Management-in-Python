# Credit acceptance rates

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Credit acceptance rates
</aside>

- These new values of loan status impact the performance metrics of our model as well as the estimated financial impact on the portfolio.

![image.png](image%2051.png)

- the threshold is used to determine what is a default or non-default, it can also be used to approve or deny new loans as they come in.
- Acceptance rate: this is a percentage of new loans that we accept with the goal of keeping the number of defaults in a portfolio below a certain number. 
** It is not a goal, but a tool to manage risk, driven by credit quality, portfolio targets, and ongoing monitoring.

![image.png](image%2052.png)

- Example
    - if we want to accept 85% of all loans with the lowest probabilities of default, then our acceptance rate is 85%.
    
    ![image.png](image%2053.png)
    
    - this means we reject 15% of all loans with the highest probabilities of default.
    - Instead of setting a threshold value, we want to calculate it to separate the loans we accept using our acceptance rate from the loans we reject.
    - in order to calculate this threshold, we need to use the quantile function from numpy.
    
    ![image.png](image%2054.png)
    
    ![image.png](image%2055.png)
    
    ** Bad rate calculation 
    
    $$
    \text{Bad Rate} = \frac{\text{Accepted Defaults}}{\text{Total Accepted Loans}}
    $$
    
    ![image.png](image%2056.png)
    
    ** Bad Rate: it is a measure of how risky your accepted portfolio is. 
    
    ** This approach is **data-driven and flexible**. In a nutshell, it says “rather than guessing a score cutoff and hoping it gives us the acceptance rate we want, let’s pick the acceptance rate (e.g., 70%) and let the data tell us what score threshold achieves that.”
    
    ** pd.crosstab(X, Y): X goes to the vertical line, Y goes to the horizontal line.