# The Capital Asset Pricing Model

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- The Capital Asset Pricing model
</aside>

- Factor analysis is the practice of using known factors such as the returns of large stocks or growth stocks as independent variables in your analysis of portfolio returns, and there are many different factor models.
    - the Capital Asset Pricing Model(CAPM):
        - excess returns: to calculate excess returns, simply subtract the risk free rate of return from your total return
        
        ![image.png](image%2037.png)
        
        - The Capital Asset Pricing Model: the cornerstone of many different financial formulas. CAPM relies on a single important factor, beta. Beta is your exposure to a regional broad market benchmark portfolio.
        
        ![image.png](image%2038.png)
        
        A high beta means a high market exposure, a low or even negative beta means low or negative exposure to market movements. 
        
        - Calculating Beta using co-variance
        
        ![image.png](image%2039.png)
        
        this approach doesn’t allow for additional factors to be easily incorporated into the analysis.
        
        ![image.png](image%2040.png)
        
        - Linear regression: a common way to analyze the impact of independent variables, or factors, on a dependent variable.
            
            ![image.png](image%2041.png)
            
        
        ** Beta in the formula is simply the coefficient of this regression.
        
        ![image.png](image%2042.png)
        
        ![image.png](image%2043.png)
        
        ** R squared value: a measure of the percent of variance of the regressed variable explained by the regressor factors, ranging from 0 to 100%.