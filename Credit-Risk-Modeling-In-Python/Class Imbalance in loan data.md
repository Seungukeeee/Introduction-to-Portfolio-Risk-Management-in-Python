# Class Imbalance in loan data

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Class imbalance in loan data
</aside>

- the nubmer of classes are often unbalanced in datasets.

![image.png](image%2029.png)

- our tree models use a loss function called log-loss. our model wants to predict both classes accurately as this leads to an overall better score.

![image.png](image%2030.png)

The problem is, for loans, a default predicted to be a non-default is much more costly. 

![image.png](image%2031.png)

- Causes of imbalance
    - data problems
    - business processes
    - behavioral factors
- dealing with class imbalance

![image.png](image%2032.png)

- Undersampling strategy
    - it is to take a random sample of non-defaults and combine it with our defaults.
    
    ![image.png](image%2033.png)
    
    ![image.png](image%2034.png)
    
    ![image.png](image%2035.png)