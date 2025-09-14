# Risk with missing data in loan data

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Risk with missing data in loan data
</aside>

- What is missing data?
    - NULLs in a row instead of an actual value.
    - An empty string ‘’ .
    - it can occur in any column in the data .
- Similarities with outliers
    - negatively affect machine leraning model performance.
    - it can bias our model in unanticipated ways, which can affect how we predict defaults.
- How to handle missing data
    - Replace values where the data is missing with the average value of that column.
    - Remove the row with missing dtaa all together.
    - Leave the rows with missing data unchanged.
- Finding missing data
    - isnull() function
    - sum() function
    - .any() method
- Replacing missing data
    - .fillna() function
    
    ![image.png](image%204.png)
    
- Dropping missing data
    - .drop() method
    
    ![image.png](image%205.png)