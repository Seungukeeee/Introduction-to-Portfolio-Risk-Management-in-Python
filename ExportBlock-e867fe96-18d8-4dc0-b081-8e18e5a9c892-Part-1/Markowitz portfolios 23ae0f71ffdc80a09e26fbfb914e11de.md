# Markowitz portfolios

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Markowitz portfolios
</aside>

- Imagine you have 9 assets, and have randomly generated 100 thousand different portfolio examples, each with different weights, and different levels of risk and return. In order to **compare portfolio performance,** you’ll want to **take into account risk-adjusted returns**.
    - Sharpe ratio is a useful metric which is quoted quite frequently in finance for this purpose.
    
    ![image.png](image%2030.png)
    
    it measures **how much return an investor can expect for each incremental unit of risk, and thus can be used to compare portfolios with different levels of risk.** This formula assumes **risk-free rate of return.** 
    
    - Efficient frontier: it gives you the highest expected return for a given level of risk.
    
    ![image.png](image%2031.png)
    
    you can select the **tangency portfolio, which is the portfolio with the highest sharpe ratio and crosses the capital allocation line according to the CAPM theory.** 
    
    - The Markowitz portfolios: The tangency portfolio is known as the max sharpe ratio, or MSR portfolio. The GMV, or global minimum volatility portfolio, is the portfolio on the far left edge of the plot with the lowest volatility.
    
    ![image.png](image%2032.png)
    
    both the MSR and GMV are known as Markowitz portfolios. the closer you are to the efficient frontier, the green line, the better the portfolio. The place where the capital association line hits 0 on the x-axis, that would be the risk free rate.
    
    ** Note that any portfolio below the efficient frontier is technically sub-par(meaning below the expected standard) compared to other possible portfolios.
    
    ** Choosing a point on the efficient frontier is a matter of personal preference.
    
    ![image.png](image%2033.png)
    
    ![image.png](image%2034.png)