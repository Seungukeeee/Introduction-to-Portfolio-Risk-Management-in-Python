# Volatility and extreme values

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Volatility and extreme values
</aside>

- Visually identifying the exact moment of a structural break is often not possible, due to noise in the data. The trend of the data may not reveal a distribution change.
- one way to address this is **to examine if times of structural change coincide with times of increased volatility**.
    - After all, change is often accompanied by greater uncertainty about the future, and this translates into more volatility.
    - Examining volatility also allows for a richer class of risk factor models to be applied and tested, such as the stochastic volatility models commonly used in asset pricing.
- Rolling window volatility
    - we can see if volatility is non-stationary by constructing a rolling window of losses (or returns) and computing the volatility for each window.
    
    ![image.png](image%2061.png)
    
    - Ploting the resulting volatility series can help identify dates where the volatility appeared to change significantly.
    
    ![image.png](image%2062.png)
    
- Extreme values
    - a second method of identifying structural breaks uses the same concepts as VaR and CVaR.
    
    ![image.png](image%2063.png)
    
    ![image.png](image%2064.png)