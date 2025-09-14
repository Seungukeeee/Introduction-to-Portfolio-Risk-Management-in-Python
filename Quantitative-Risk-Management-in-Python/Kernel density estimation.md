# Kernel density estimation

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Kernel density estimation
</aside>

- up to now, our risk factor distributions have been assumed (such as the Normal or T distribution), fitted or ignored.
- A middle ground between parametric estimation and ignoring the distribution is to filter the data so that they become smooth enough to represent a distribution. This can be done with non-parametric estimation, which does not assume a parametrized class of distributions (such as the Normal, skewed normal, or Student’s t-distribution).
- The idea behind a filter is **to smoothen out the bumps of a histogram**, so that a function can be fit to the histogram data.

![image.png](image%2071.png)

- The Gaussian kernel
    - This is a continuous kernel that puts the selected portfolio value at the center of a Normal distribution, and then **weighs neighboring values according to how far away they are from the center**.
    - There are in general many kernels that can be used to fit a given set of observations.
    - Kernel density estimation is extensively used in time series analysis, signal processing, and many other problem areas.
    
    ![image.png](image%2072.png)
    
    ![image.png](image%2073.png)
    
    ![image.png](image%2074.png)