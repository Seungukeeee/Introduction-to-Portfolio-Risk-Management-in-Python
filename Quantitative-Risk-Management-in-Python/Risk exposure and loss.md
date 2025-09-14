# Risk exposure and loss

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Risk exposure and loss
</aside>

- Risk exposure and VaR
    - Risk exposure: the product of the probability of an event causing a loss, multiplied by the amount of a loss if one should occur.
        - Loss measure: e.g. VaR (it is the minimum amount ‘in danger’ of being lost at the VaR’s confidence level.
        
        ![image.png](image%2018.png)
        
        ![image.png](image%2019.png)
        
        ** Note that the 90% confidence level is derived from 100% - the actual probability of loss in our example.
        
        ![image.png](image%2020.png)
        
        ** how do you choose between the two options? the final variable is the difference in hotel price, 50 euros (the basic price difference). This is more than the difference in risk exposures, 39 euros. So the hotel’s two options are asking you about **your risk tolerance**: is it worth paying 50 euros more to avoid a greater risk exposure of 39 euros?
        
        → you’re likely risk-neutral if you prefer the non-refundable option over the partially refundable option. Since the 39 euros difference is less than the payment of 50 euros to avoid the greater risk exposure, risk neutrality implies you’ll select the non-refundable option.  you’re likely risk-averse if you prefer the partially refundable option. You pay the 50 euros to avoid the risk of losing 39 euros, because uncertainty is costly. **This measurement of costliness expresses risk preference**.
        
        - Enterprise risk preference is called **risk appetite**
        - individual investors risk preference is called **risk tolerance**.
        
        ![image.png](image%2021.png)
        
        ![image.png](image%2022.png)
        
        ![image.png](image%2023.png)
        
        ![image.png](image%2024.png)
        
        ### **Risk interpretation**
        
        - **€50** means: *Given a 10% chance of illness, your expected “at-risk” amount is €50 under the non-refundable plan.*
        - **€11** means: *Same probability, but much lower exposure with partial refund.*
        - The difference (€39) is essentially **the risk reduction** from choosing partial refund coverage.