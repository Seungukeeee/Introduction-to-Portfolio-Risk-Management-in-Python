# Parametric Estimation

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- How to estimate risk measures by fitting distributions to data.
</aside>

- Generally, we do not know the exact form of the distribution of possible losses.
    - A class of distributions
        - each member of a class is a function of the loss ‘x’ and has a set of parameters, which we call ‘theta’.
            - e.g. a Normal distribution is a class of distributions, each with a different mean and standard deviation.
        - Finding the ‘best’ parameter values given portfolio data is called **parametric estimation**.
        
        ![image.png](image%2047.png)
        
        Once the optimal parameter values ‘theta star’ are found, the loss distribution can be described within the class of distributions. 
        
    - Fitting a distribution
        - this fitting usually involves trying to bend the shape of the class so that it minimizes some measurement of error.
            - e.g. the ‘fit()’ method of Scipy’s normal distribution does this by selecting the best mean and standard deviation for error minimization.
        - This provides a way to visually compare the fitted distribution and a histogram of the data.
        - it also allows us to use statistical inference to measure goodness of fit.
        
        ![image.png](image%2048.png)
        
        ![image.png](image%2049.png)
        
    - Anderson-Darling test
        - Sometimes a visualization will make it appear that a distribution is a good fit. How can we make this precise?
            - The Anderson-Darling test is used to see how well a distribution fits the data.
            - The null hypothesis is that the data are Normally distributed.
            - This is rejected if the test statistic comes back larger than one or more critical values (just like a t-test from OLS).
        
        ![image.png](image%2050.png)
        
    - Skewness
        - Skewness is the degree to which data is non-symetrically distributed, such as the normal distribution, or the T distribution, cannot account for skewness.
        - The Skewed Normal distribution is a generalization of the Normal distribution, can be asymmetric.
        - This is very useful for portfolio data, where losses and gains may not be symmetrically distributed.
        
        ![image.png](image%2051.png)
        
    - Testing for skewness
        - it tests by seeing how far data are from being symmetric.
        - The null hypothesis is that there is no skewness, indicating the a symmetric distribution is appropriate.
        
        ![image.png](image%2052.png)
        

![image.png](image%2053.png)

from the lines, to calculate VaR, there are two approaches of returning VaR value

- One is to use np.quantile.
- Another is using norm.ppf() method, putting two parmeters(the quantile, params)