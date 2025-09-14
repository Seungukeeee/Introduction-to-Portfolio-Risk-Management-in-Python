# Credit model performance

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Credit model performance
</aside>

- Accuracy
    - it is the number of correct predictions divided by the total number of predictions.
    
    ![image.png](image%206.png)
    
- ROC curve(Receiver Operating Characteristic curve)
    - it plots true positive rate (sensitivity) against false positive rate (Fall-out, the percentage of incorrectly predicted defaults).
    
    ![image.png](image%207.png)
    
    - ROC charts are interpreted by looking at how far away the model’s curve gets from the dotted blue line.
    - AUC is the calculated area between the curve and the random prediction. This is a direct indicator of how well our model makes predictions.
    
    ![image.png](image%208.png)
    
- Default thresholds: to analyze performance further, we need to decide what probability range is a default, and what is a non-default.

![image.png](image%209.png)

![image.png](image%2010.png)

![image.png](image%2011.png)

![image.png](image%2012.png)