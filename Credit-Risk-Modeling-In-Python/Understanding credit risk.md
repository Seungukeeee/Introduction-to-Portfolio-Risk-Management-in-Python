# Understanding credit risk

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Understanding credit risk
</aside>

- What is credit risk?
    - Credit risk is **the risk that someone who has borrowed money will not repay it all.**  Think of this risk as the difference between lending money to a person and purchasing a government bond.
    - A loan is in default when the lending agency is reasonably certain the loan will not be repaid.
    - Expected loss: the amount that the firm loses as a result of the default on a loan. Expected loss is a simple calculation of the following three components.
        - The probability of Default (PD): The likelihood that someone will default on a loan.
        - The Exposure at Default (EAD): the amount oustanding at the time of default.
        - The loss given default (LGD): the ratio of the exposure against any recovery from the loss.
        
        $$
        \text{Expected Loss} = \text{PD} \times \text{EAD} \times \text{LGD}
        $$
        
- Types of data used
    - Application data: data that is directly tied to the loan application like loan grade.
    - Behavioral data: data that describes the recipient of the loan, such as employment length.
    
    ![image.png](image%201.png)
    
- Exploring with cross tables: it helps get a high level view of the data similar to pivot tables in Excel.

![image.png](image%202.png)

- Practice
    - 
    
    ![image.png](image%203.png)
    
    the average percentage of income for defaults is higher. This could indicate those recipients have a **debt-to-income ratio that’s already too high**.
    
    ** Debt-to-income ratio? a financial metric that compares how much you owe each month to how much you earn. It's a percentage that lenders use to assess your ability to manage monthly debt payments and repay new loans (from [https://www.discover.com/home-loans/articles/understanding-debt-to-income-ratio/](https://www.discover.com/home-loans/articles/understanding-debt-to-income-ratio/))