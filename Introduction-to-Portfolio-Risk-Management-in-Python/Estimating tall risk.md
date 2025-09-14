# Estimating tall risk

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Estimating tall risk
</aside>

- A key component of portfolio risk management is being able to define risk beyond simple measures such as standard deviation, variance, and even kurtosis. More important is the ability to quantify potential losses on a single stock and portfolio level.
    - Tail risk: it is essentially the risk of extreme outcomes in the tail of the return distribution, particularly in the left tail, which signifies an extremely negative return.
        - Historical drawdown: it is a way to estimate the percentage loss from the highest point. in other words, haw far have you fallen from your best point in history?
        
        ![image.png](image%2052.png)
        
        ![image.png](image%2053.png)
        
        This is your drawdown, and as you can see, it will never rise above 0. 
        
        - Value at Risk(VaR): a way to estimate the risk of a single day negative price movement. VaR always has a quantile, or percentage attached to it. For example, a VaR 95 of -2.3% means in the worst 5% of scenarios, my losses will exceed -2.3%.
            
            ![image.png](image%2054.png)
            
            ![image.png](image%2055.png)
            
        - Historical expected shrtfall(Conditional Value at Risk): a measure of the expected value of losses in the worst 1 minus x percent of scenarios, which is where the alternatvie name “expected shortfall” is derived from.
        
        ![image.png](image%2056.png)
        
        In this example, CVaR(95) = -2.5% means that in the worst 100 - 95, or the worst 95% of cases, losses will be on average on -2.5%. This is essentially the same as taking the average of losses exceeding the VaR(95) level. 
        
        ![image.png](image%2057.png)