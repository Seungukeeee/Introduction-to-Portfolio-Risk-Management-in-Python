# Measuring Risk

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Measuring Risk
</aside>

- we’ll estimate how much a portfolio stands to lose, using the Value at Risk and Conditional Value at Risk statistics.
- The Loss distribution
    
    ![image.png](image%2011.png)
    
    - A loss distribution tells us a portfolio’s future potential losses due to the random nature of its risk factors, when holdings are fixed over a time horizon.
- Maximum loss
    - for financial instituions, an upper bound on losses is crucial. Because risk factors are random, it is usually not possible to bound losses with 100% certainty. Instead, we look for **the likelihood that losses will remain capped by an upper bound**. This likelihood is called **the confidence level**. The confidence level allows us to express questions about the maximum loss from a likelihood perspective, such as “what is the maximum loss that would take place 95% of the time?”
        
        ![image.png](image%2012.png)
        
- Value at Risk (VaR)
    - it measures **the maximum portfolio loss for a given confidence level**.
        - VaR is usually expressed for 95%, or 99.5% confidence levels.
        
        ![image.png](image%2013.png)
        
- Conditional Value at Risk (CVaR)
    - it measures **expected loss given a minimum loss equal to the VaR**.
    - CVaR is the expected value of the loss over the tail of the loss distribution.
    
    ** Note that CVaR is sometimes expressed using the confidence level, 95%, and sometimes, with the significance level, which is 100% - the confidence level. 
    
    ![image.png](image%2014.png)
    
    - Computing the CVaR requires the loss distribution, the maximum possible loss (which may be infinite), and the minimum possible loss (which is the VaR).
- Deriving the VaR
    - Specify confidence level, e.g. 95% (0.95)
    - create series of loss observations.
    - compute loss.quantile() at specified confidence level.
    - VaR = computed .quantile() at desired confidence level.
    - scipy.stats loss distribution: percent point function .ppt() can also be used.

![image.png](image%2015.png)

- Deriving the CVaR
    - Specify confidence level, e.g. 95% (0.95)
    - Create or use sample from loss distribution.
    - Compute VaR at a specified confidence level, e.g. 0.95.
    - Compute CVaR as expected loss (Normal distribution: scipy.stats.norm.expect() does this).
    
    ![image.png](image%2016.png)
    
- Visualizing the VaR
    
    ![image.png](image%2017.png)