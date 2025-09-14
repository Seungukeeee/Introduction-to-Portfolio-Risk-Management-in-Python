# Mean, variance, and normal distribution

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Mean, variance, and normal distribution
</aside>

- financial risk can simply be thought of as a measure of uncertainty of future returns.
- Probability distributions have the following moments
    - Mean (mu)
    - Variance (sigma): a measure of the variability in outcomes.
    - Skewness: a measure of the “tilt” of a distribution.
    - Kurtosis: a measure of the thickness of the tails of a distribution.
- The standard normal distribution: a special case of the normal distribution when sigma = 1, mu = 0.
    - All normal distributions tend to have a skewness near 0 and a kurtosis near 3.
        - Financial returns tend to have positive skewness and a kurtosis higher than 3. This means financial returns tend to have a higher probability of both outliers and of positive returns than a normal distribution.
        
        ![image.png](image%2011.png)
        
        - there are statistical tests for normality(such as Shapiro-Wilk, Jarque-Bera), but a high kurtosis or large skewness is a simple indicator of non-normal returns.
        
        ![image.png](image%2012.png)
        
        if you want to annualize that number, you’ll first need to add 1 to the decimal before raising the quantity to the power of 252, which is the typical number of trading days in a year. For example, a daily return of just 0.03% works out to an annualized return of 7.85% when it is compounded every day for 252 trading days in a row.
        
    - The second moment of the distribution, the variance, volatility is one of the most important concepts for risk management in finance. The fundamental takeaway is simple: **an investment with higher volatility is viewed as a higher risk investment**.
        - Volatility is another measure of the dispersion of returns, just like variance.
        
        ![image.png](image%2013.png)
        
    - it is very important to understand that **volatility scales with the square root of time**. To properly scale the daily volatility of an asset, simply multiply the volatility by the square root of the number of trading days in a year.

![image.png](image%2014.png)

![image.png](image%2015.png)