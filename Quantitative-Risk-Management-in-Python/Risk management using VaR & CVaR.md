# Risk management using VaR & CVaR

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Risk management using VaR & CVaR
</aside>

![image.png](image%2025.png)

- Modern portfolio theory is also called mean-variance portfolio optimization as it asks for the highest expected return, given our level of risk expressed as a variance.
- By contrast, the VaR and CVaR risk measures address how much we expect to lose and not just a particular risk level.

![image.png](image%2026.png)

- We do this by changing the objective function of the optimization problem: **instead of looking for the portfolio weights that maximize the expected portfolio return, we look for the portfolio weights that minimize the expected conditional loss at some confidence level**.

![image.png](image%2027.png)

- The risk management problem
    - it selects optimal portfolio weights w* (w-start) as solution to minimize the CVaR, given a confidence level ‘alpha’.
    
    ![image.png](image%2028.png)
    
    ** ‘x’ is the portfolio loss, and depends upon the weights ‘w’. Loss is the negative of returns, and its distribution ‘f(x)’ is calculated from a numerical estimate. 
    
    ** As always, the portfolio weights have to sum up to one. 
    
    ![image.png](image%2029.png)
    
    ![image.png](image%2030.png)
    
    ![image.png](image%2031.png)
    

![image.png](image%2032.png)