# Gradient boosted trees with XG Boost

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Gradient boosted trees with XGBoost
</aside>

- Decision trees
    - it creates predictions similar to logistic regression in a different structure.
    
    ![image.png](image%2023.png)
    
    the results of these splits are yes and no decisions that eventually lead to a predicted loan status of default or non-default. 
    
    ![image.png](image%2024.png)
    
    the consequence of two wrong predictions(predicted default for non-default cases) leads to a loss of 2200 worth.
    
- XG Boost

![image.png](image%2025.png)

![image.png](image%2026.png)

![image.png](image%2027.png)

** np.ravel(): it is a function to convert the shape of input data into 1-d array. since its function changes the input data shape itself, it doesn’t need extra memory to save the copy of it.

** np.flatten(): it has the same function as np.ravel(), but it stores a copy of the original input data. therefore, it needs more memory for implementing it. 

- Hyperparameters of gradient boosted trees
    - hyperparameters cannot be learned from data; they have to be set by us.

![image.png](image%2028.png)

- Expected Loss: it represents the average loss a lender expects to incur over a specific time horizon (typically one year) due to borrower defaults. It can be calculated in the following …
    
    $$
    Expected Loss (EL)=PD×LGD×EAD
    $$
    
    - Probability of Default (PD): it is the likelihood that a borrower will default on their debt obligations over a given time horizon (often 1 year).
        - Expressed as a percentage (e.g., 2% chance of default).
        - Based on internal credit rating models, historical data, or market-based indicators.
    - Loss Given Default (LGD): it is the proportion of the exposure that a lender loses if the borrower defaults, after accounting for recoveries (like collateral or bankruptcy proceedings)
        - Expressed as a percentage (e.g., 40% means you lose 40% of the loan)
        - LGD = 1 - Recovery Rate
    - Exposure at Default (EAD): it is the total value a lender is exposed to when a borrower defaults. It includes the current outstanding amount and possibly undrawn credit lines.
        - For loans: typically the oustanding loan balance
        - For revolving credit (e.g., credit cards): includes estimated future drawdowns.