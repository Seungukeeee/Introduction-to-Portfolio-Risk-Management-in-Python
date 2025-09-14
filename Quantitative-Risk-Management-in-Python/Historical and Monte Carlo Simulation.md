# Historical and Monte Carlo Simulation

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Hsitorical and Monte Carlo Simulation
</aside>

- Historical simulation
    - Historical simulation uses past data to create a simulation about the future loss.
    - It makes **no assumption about the loss distribution shape**.
    - If we have a vector of losses stretching back, say, 365 days, then we create a vector of 365 simulated losses from today onwards by using past losses as if they occurred today.
    
    ![image.png](image%2041.png)
    
    ![image.png](image%2042.png)
    
    ** The generality of historical simulation is also its weakness. it may not be true that the loss distribution is stable over time, especially during times of structural changes (such as the financial crisis). 
    
- Monte Carlo simulation
    - it is a technique that combines aspects of both parametric and historical simulation.
    - it starts with a particular distribution class for losses or risk factors.
    - It uses the distribution to create a series of random draws.
    - it simulates a path of losses over time. Once this is done for a single path, or run, the process is repeated with a new series of random draws, to create a set of runs.
    - each run generates a simulated loss.
    - The VaR estimate is then computed as a quantile over these losses, so that the entire set of runs is treated as a distribution of losses.
    
    ![image.png](image%2043.png)
    
    ![image.png](image%2044.png)
    
    ![image.png](image%2045.png)
    
- Simulating asset returns
    - refinement: generate random sample paths of asset returns in portfolio.
    - this allows greater realism as each risk factor can contribute their own sample path.
    - in addition, risk factors can be correlated: the covariance maxtrix can be used to compute asset returns in the simulation procedure.
    
    ![image.png](image%2046.png)