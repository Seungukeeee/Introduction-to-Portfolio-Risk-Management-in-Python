# Structural breaks

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Structural breaks
</aside>

- our main tool for risk mitigation is Modern Portfolio Theory

![image.png](image%2054.png)

- Stationarity
    - This connection also assumes that the underlying distribution is the same over the time the risk factor data is collected. In otehr words, the loss(or returns) distribution is stationary.
    - it poses a problem for our estimation of risk, because all three estimation procedures we discussed assume stationary distributions.
    
    ![image.png](image%2055.png)
    
- Structural breaks
    - If we knew that **the distribution was changing over time**, and we knew when distribution changes occur, then we could estimate our risk measures only during sub-periods when the distribution didn’t change. In other words, distributions would be stationary only within certain sub-periods of the data.
        - we first need to know when the data suggest that an underlying distribution is changing.
        - This is the known as a “structural break” point in the data.
        - you can think of a structural break as a change in a “trend”.
        
        ![image.png](image%2056.png)
        

![image.png](image%2057.png)

- The Chow test
    - there is a powerful statistical tools that can be applied to data(to see the structural breaks).
    - Chow Test: it asks if the data support a structural break at a given break point of time, **for a given linear risk factor model**.
    - Its null hypothesis: no structural break(the trend has “no change”).
    - in the test, three ordinary least squares regressions are performed
        - Regression for entire period
        - Two regressions, before and after break.
    - The sum of squared residuals are then collected, and the Chow test statistic is created.
    - The statistic is distributed as an “F”-distribution statistic.
    
    ![image.png](image%2058.png)
    
    ![image.png](image%2059.png)
    
    ![image.png](image%2060.png)