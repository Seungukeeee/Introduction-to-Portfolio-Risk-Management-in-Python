# Column selection for credit risk

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Column selection for credit risk
</aside>

- Column importances
    - Use the .get_booster() and .get_score() methods (for checking the feature importance).
        - weight: the number of times the column appears in all trees.
        
        ![image.png](image%2041.png)
        
        - Plotting column importances
        
        ![image.png](image%2042.png)
        
    
    - once we have the importances for each column, to determine if we want to create a new training set with only select columns.
    
    ![image.png](image%2043.png)
    
    sometime adding more columns increases accuracy, but it can also make it more difficult for the model to learn and decrease other performance metrics like default recall. 
    
    - F1 scoring for models
    
    ![image.png](image%2044.png)
    
    this is useful as it helps us keep recall for loan defaults as an important consideration for any model.