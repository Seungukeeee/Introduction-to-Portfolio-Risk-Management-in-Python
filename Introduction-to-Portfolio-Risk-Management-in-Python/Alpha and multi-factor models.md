# Alpha and multi-factor models

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Alpha and multi-factor models
</aside>

- The Fama-French 3 factor Model
    - one of the most widely used model in finance for portfolio management.
    
    ![image.png](image%2044.png)
    
    this model extends the CAPM model by adding the SMB, or size factor, as well as the HML, or value factor.  HML stands for high minus low, whereas the acronym for size, SMB, stands for small minus big. This is because **small stocks tend to outperform big stocks, so small stock returns minus big stock returns is essentially the small size premium.** Value versus growth, or high minus low, on the other hand, is more cyclical. For example, during the crisis, value stocks outperformed, but during bull runs, growth stocks sometimes outperform.
    
    ![image.png](image%2045.png)
    
    - P-values and statistical significance
    
    ![image.png](image%2046.png)
    
    ![image.png](image%2047.png)
    
    - Alpha and the efficient market hypothesis: Anything that couldn’t be explained by the beta, size, or value factors in the model is called alpha, which is essentially **an error term**. Positive alpha is now popularly interpreted as outperformance due to skill, luck, or timing. **for every fund with positive alpha, there is another fund with negative alpha since the weighted sum of all apha in a market must be 0**. This is because the weighted sum of the returns of all investors simply equals the market portfolio.
        - The efficient market hypothesis states that the market prices all information. Therefore, any perceived “alpha” is simply the result of a missing factor in an a more complex economic pricing model.
    
    ![image.png](image%2048.png)
    

**Interpreting p-values:**

- A p-value **less than 0.05** usually means the coefficient is **statistically significant** — i.e., there's a high likelihood the relationship isn’t due to random chance.

### 🧩 So What Does the SMB Coefficient Tell You?

**SMB** stands for **"Small Minus Big"**, and it’s a factor used in models like the **Fama-French 3-factor model**.

- If the **SMB coefficient is positive** and **statistically significant**, it means:
    
    > Your portfolio’s returns tend to behave like small-cap stocks — it’s more exposed to smaller companies.
    > 
- If the **SMB coefficient is negative** and **significant**, it means:
    
    > Your portfolio behaves more like large-cap stocks — more exposure to bigger, established companies.
    >