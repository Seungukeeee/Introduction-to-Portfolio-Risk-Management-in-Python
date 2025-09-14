# Extreme value theory

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Extreme value theory
</aside>

- Extreme value theory
    - a statistical distribution of extreme values. in other words, it is a way to help model the tail of the loss distribution.
    - Block maxima
        - the idea is to take data over a time period, break up that period into sub-periods, called blocks, and look at the maximum loss in each block.
    - Peak over threshold(POT)
        - it makes all losses above a given level the dataset of interest.
        
        ![image.png](image%2065.png)
        
- Generalized Extreme Value Distribution
    - example: Block maxima for 2007-2009
        - it resamples losses with desired period (e.g. weekly). this is a new dataset of extreme values, and can be approximated with a new distribution.
        - This distribution is the generalized extreme value distribution, or GEV.
        - We can fit the GEV distribution to our ‘maxima’ data using the ‘genextreme’ distribution from ‘scipy stats.’
        
        ![image.png](image%2066.png)
        
        - VaR and CVaR from GEV distribution
        
        ![image.png](image%2067.png)
        
        - Covering losses
            - The VaR or CVaR estimate over extreme values is often used in the banking and insurance sectors to cover losses, which is an integral part of enterprise risk management.
            - it is a regulatory requirement that banks keep enough reserves (sometimes called a reserve requirement) on hand to cover losses over a particular period at a particular confidence lvel.
            
            ![image.png](image%2068.png)
            
            ![image.png](image%2069.png)
            
            ![image.png](image%2070.png)