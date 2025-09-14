# Cross validation for credit models

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Cross validation for credit models
</aside>

- How to test our models
    - cross validation: a method for training and testing a model multiple times on the same data.
    - Within XG Boost, to use cross validation, you need to create a specialized object called DMatrix, which is a different way of storing the training data.
    - Early stopping: it tells cross validation to stop after a scoring metric has not improved after a number of iterations.
- How cross validation works
    - processes parts of training data called folds and tests against unused part.
    - final testing against the actual test set.
    
    ![image.png](image%2036.png)
    
    once this is done, the parameters are averaged across each training session and then the model is finally tested against the origianl test set.
    
- setting up cross validation within XG Boost
    - set the number of folds, early stopping, and any specific parameters for cross validation.
    - ‘binary’:’logistic’ is used to specify classification for loan_status.
    - ‘eval_metric’:’auc’ is the area under the curve.
    
    ![image.png](image%2037.png)
    
    - After creating the dictionary of parameters, we transform our training data into the specialized DMatrix object for xgboost.
    - CV function: we pass the data inthe function with all the parameters dictionary.
        
        ![image.png](image%2038.png)
        
    
    ![image.png](image%2039.png)
    
    - the CV function produces a data frame of training and test AUC scores for our models. This of this as a scenario analysis where we want to see how our model would perform as new loans come in.
- Another way of using cross validation scoring
    - cross_val_score() from scikit-learn.
    
    ![image.png](image%2040.png)