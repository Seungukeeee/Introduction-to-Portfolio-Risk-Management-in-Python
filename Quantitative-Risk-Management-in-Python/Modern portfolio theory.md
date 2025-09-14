# Modern portfolio theory

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Modern portfolio theory
</aside>

- we cannot generally guarantee a return: we can only speak about an expectation.
    - one expected return meausre: the average (mean) historical return over time. this is a proxy for future returns.
- Efficient portfolio
    - portfolio with heights generating highest expected return for given level of risk. this mathmatical way of quantifying the risk-return trade-off is called “Modern Portfolio Theory”.
    - The efficient portfolio is the solution to an optimization problem, which selects portfolio weigths to maximize the expected portfolio return, conditional upon a particular risk level given by the portfolio’s volatility.
    
    ![image.png](image%207.png)
    
- The efficient frontier
    - it computes many efficient portfolios for different levels of risk.
    - it is locus of (risk, return) pairs created by efficient portfolios.
    
    ![image.png](image%208.png)
    
    ![image.png](image%209.png)
    
    this provides, in addition to portfolio weights, risk and return values within the ‘vol’ and ‘ret’ variables, respectively. 
    
    ** To compute the efficient frontier, both expected returns and the covariance matrix of the portfolio are required. 
    
    ![image.png](image%2010.png)
    
    ** the red dot point is the minimum variance portfolio, and is often used as a benchmark to assess an investor’s risk appetite. 
    
    ```python
    from pypfopt.expected_returns import mean_historical_return
    
    mean_returns = mean_historical_return(dataframe, frequency = 252)
    ```
    
    the above code helps you get the annualized mean return (it shows the average yearly performance).
    
     
    
    ```python
    from pypfopt.risk_models import CovarianceShrinkage
    
    cs = CovarianceShrinkage(dataframe)
    ```
    
    Portfolio optimization relies upon an unbiased and efficient estimate of asset covariance. if datasets contain extreme cases, it tends to be overweighted. therefore, you need to alleviate them. One of the ways is using **covariance shrinkage**, where large errors are reduced(’shunk’) to improve efficiency. Note that although the CovarianceShrinkage object takes prices as input, it actually calculates the covariance matrix of asset returns, not prices. 
    
    its purpose is to provide a shrinkage estimator for the covariance matrix of returns. This helps reduce estimatino error, especially when you have:
    
    - Many assets
    - Limited historical data
    - Highly volatile or noisy returns