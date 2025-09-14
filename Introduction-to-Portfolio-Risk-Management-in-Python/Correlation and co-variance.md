# Correlation and co-variance

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Correlation and co-variance
</aside>

- Modern portfolio theory teaches that you can actually build a portfolio of assets which has less risk than any of the underlying assets alone because of correlation and co-variance.
    - Pearson correlation: a measure of the linear correlation between two variables, in our case, between the returns of two stocks. It ranges from -1 to 1 where 1 is perfect positive correlation, -1 would be perfect negative correlation, and 0 would be no correlation.
    
    ![image.png](image%2022.png)
    
    You can calculate the correlation coeficient for every pair of stocks in your portfolio, and this results in a matrix of correlations.
    
    ![image.png](image%2023.png)
    
    - Portfolio standard deviation
    
    ![image.png](image%2024.png)
    
    ![image.png](image%2025.png)
    
    correlation is a normalized measure of the co-variance. Co-variance measures the joint variability of two random variables, and in finance, the co-variance matrix is often used for portfolio optimization and risk management purposes.
    
    ![image.png](image%2026.png)
    
    the variance of a stock scales linearly with time, or the volatility with the square root of time.
    
    ![image.png](image%2027.png)
    
    ![image.png](image%2028.png)
    
    ![image.png](image%2029.png)
    

### 🎯 Real-Life Use Flow:

1. **Use correlation** to:
    - Explore which assets **diversify each other well**.
    - Spot relationships like: “Tech and gold have low correlation.”
    - Make initial **portfolio design** choices.
2. **Use covariance** to:
    - Plug into the **portfolio variance formula** (risk).
    - Quantify the actual **risk impact** of those relationships, given your specific **asset weights** and **return volatilities**.
    - Help in building things like the **efficient frontier**.

** basically, correlation and covariance work in the same way, which is used to check the relationship between variables. but correlation is calculated in a standardized unit, but covariance is measured in its actual unit. therefore, one way suggests that using correlation is effective when measuring the relative relationship, using covariance is more helpful when estimating the range of loss and profit.

## 📊 Understanding Annualized Volatility: Fixed vs. Dynamic

In most financial tutorials and models, **volatility is often annualized** using the following formula:

```

Annualized Volatility = Daily Volatility × √252
```

This works under the assumption that **volatility is constant over time**, which makes comparison across assets or strategies simpler. However, in reality, **market volatility fluctuates constantly** due to changing economic conditions, news, investor sentiment, and more.

---

## ⚠️ The Problem with a Single Fixed Estimate

Relying on **one fixed annual volatility number** can be overly simplistic and even misleading. Volatility behaves more like a **living, breathing variable** — some periods are calm, others are turbulent.

To reflect this reality more accurately, it’s often better to use a **range** or **time series of annualized volatility** estimates instead of a single figure.

---

## ✅ A More Realistic Approach: Rolling Volatility

One way to capture changing volatility is to calculate **rolling volatility**:

- Compute **daily or weekly rolling standard deviations** of returns (e.g., 30-day windows).
- Multiply each by √252 to convert to annualized volatility.
- This gives you a **time series of annualized volatility**, which better reflects how risk evolves over time.

You can then summarize it as:

- Minimum annualized volatility over the period
- Maximum (peak stress level)
- Average (baseline expectation)

This gives your analysis more depth and makes your backtesting or risk modeling much more grounded in reality.

---

## 💬 Why It Matters

By using a **range of possible volatilities**:

- You acknowledge that **risk is not constant**.
- You can **stress-test** your portfolio against historical extremes.
- You make **more informed decisions** about position sizing, rebalancing, and drawdown expectations.