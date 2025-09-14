# VaR extensions

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- VaR extensions
</aside>

- VaR quantiles: the higher the quantile, the higher the potential losses, and sometimes quite dramatically higher. This can lead to over-estimating risk, which can cause you to lose money by being too cautious. This is why testing different quantile parameters is important to striking the right balance between risk and reward.
    - Empirical assumptions: Empirical historical values are those that have actually occurred. But it still doesn’t guarantee all the possible cases. then how do you simulate the probability of a value that has never occurred historically before?
        - One way is to assume a probability distribution and to extract values from the quantiles of this distribution.
        
        ![image.png](image%2049.png)
        
        you can use the norm.ppf function to compute the parametric VaR of a normal distribution, in this case, setting the mean and standard deviation equal to the mean and standard deviation of your historical returns. this doesn’t address the non-normality of returns, but it’s arguably more scientific than simply grabbing from a bucket of historical returns, and it allows for some flexibility when it comes to simulations. 
        
        ![image.png](image%2050.png)
        
        Since losses and returns compound, you’re going to need to scale these estimates using the square root of time. 
        
        ![image.png](image%2051.png)