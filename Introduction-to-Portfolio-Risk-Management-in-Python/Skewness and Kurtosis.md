# Skewness and Kurtosis

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Skewness and kurtosis
</aside>

- Skewness: a measure of how much a distribution leans to the left or right.
    - Negative skew: a right-leaning curve
    - Positive skew: a left learning curve.
    - in finance, you would tend to want positive skewness with a higher probability of significantly good returns on the right hand side of the distributino, and a compressed, predictable left-hand distribution of negative returns.
    
    ![image.png](image%206.png)
    
    ![image.png](image%207.png)
    
    ** Be sure to drop any NA values using the dropna() method.
    
    - Skewness above 0 indicates possible non-normality, which you can expect to find in financial returns.
- Kurtosis: a measure of the thickness of the tails of a distribution, which can be used a proxy for the probability of outliers. ** proxy: something that is used as a substitute or stand-in for something else when the actual thing is hard to measure directly.
    - Most financial returns are leptokurtic, which simply means that they tend to have positive excess kurtosis, or kurtosis greater than 3.
    - Kurtosis is often compared to a normal distribution, many functions in Python will automatically return excess kurtosis, which essentially the sample kurtosis minus 3, which helps demonstrate whether the probability of outliers is higher or lower than a normal distribution.
    
    ![image.png](image%208.png)
    
    If excess kurtosis is higher than 0, the kurtosis is higher than a normal distribution. 
    
    ![image.png](image%209.png)
    
    ** in finance, high excess kurtosis is an indication of high risk. when large movements in returns happen often, this can be a very bad thing for your portfolio if it moves in the wrong direction. 
    
    ** High kurtosis distributions are said to have “thick tails”, which means that outliers, such as extreme negative and positive returns, are more common.
    
    ![image.png](image%2010.png)