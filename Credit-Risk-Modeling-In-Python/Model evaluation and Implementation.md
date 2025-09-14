# Model evaluation and Implementation

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Model evaluation and Implementation
</aside>

- comparing classification reports
    - Macro Average: The unweighted average of the F1 score for default and non-default.
    
    ![image.png](image%2045.png)
    
    we can get a good understanding of each model’s performance across defaults and non-defaults. 
    
    - ROC and AUC analysis: the greater the lift means that the AUC score is higher and the model has better performance overall for defaults and non-defaults.
    
    ![image.png](image%2046.png)
    
    - Model calibration: it checks how well calibrated their predicted probabilities are. what this means is we want to be able to interpret these probabilities as a confidence level for default. A model is well-calibrated when a sample of loans has an average predicted probability of default close to that sample’s percentage of actual defaults.
    
    ![image.png](image%2047.png)
    
    To calculate these values, we use the calibration curve function. 
    
    ![image.png](image%2048.png)
    
    ![image.png](image%2049.png)
    

![image.png](image%2050.png)