# Portfolio hedging: offsetting risk

Type: class
Course: Quantitative Risk Management in Python (Quantitative%20Risk%20Management%20in%20Python%2023ee0f71ffdc80a88b40e5c4037cadd6.md)
Done: Done

---

<aside>

ABOUT

- Offestting risk
</aside>

- A risk measure such as VaR or CVaR indicates **potential portfolio losses**. These losses may still occur even after portfolio optimization has been performed, because of the volatility of the portfolio’s risk factors.
    - for large institutional investors, such as pension funds, portfolio stability is a key requirement because portfolio returns pay the income of individuals who have retired.

![image.png](image%2033.png)

the volatility of rain as a risk factor for sunglasses, in other words, is offset by investing in umbrellas. 

- Hedging
    - Using one or more assets to offset a risky position is called hedging.
    - it is one of the most important institutional investor techniques for risk management.
    - By hedging a portfolio, an investor finds another return stream that moves in the opposite direction to the portfolio’s risk factor.
    - Hedging is often performed using derivatives to offset a risky asset position.
    - Hedge instruments: options
        - derivative: hedge instrument
            - European option: very popular derivative
                - A European ‘call’ option gives the holder the right (but not the obligation) to purchase a stock for a fixed price X at a particular time M.
                - A European ‘put’ option gives the holder the right (but not the obligation) to sell a stock for a fixed price X at a particular time M.
                - The stock is called the ‘underlying’ of the option (the thing the ticket is about).
                - The market price of the underlying is called the ‘spot’ price ‘S’.
                - The fixed price is called the ‘strike’ price ‘X’ and the time ‘M’ is the ‘maturity’.
                
                ![image.png](image%2034.png)
                
            - Black-Scholes option pricing
                - The value of an option changes when the underlying asset price changes.
                - if this change moves opposite to the price change, then a portfolio with the asset can be hedged.
                - To value the options, many factors such as market efficiency, the underlying stock, and the risk-free interest rate all play a factor.
                - Black-Scholes option pricing formula is the most popular way.
                
                ![image.png](image%2035.png)
                
                - this formula makes some assumptions about how markets work, and how the underlying stock price evolves.
                    - the markets are well-functioning that the stock price follows a particular statistical distribution
                    - there are safe investment opportunities such as bank deposits.
                    
                    ![image.png](image%2036.png)
                    
                - To calculate the options value, a pre-generated function ‘black_scholes’ is available.
                
                ![image.png](image%2037.png)
                
            - A portfolio made up of a single stock can be hedged by holding a European put option with the same underlying stock.
                - The value of a put option goes up when the price of a stock goes down.
                - The change in the option value is called the “Delta” of the option. It is the derivative of the option value V with respect to the spot price S.
                - By holding an amount of the option equal to one over the delta, changes in the price of the undelying stock can be offset.
                - Delta neutrality is when the total change in the portfolio’s value from a change in the portfolio’s asset price is zero.
                - The function ‘bs_delta’ is used to compute the delta.
                
                ![image.png](image%2038.png)
                

![image.png](image%2039.png)

![image.png](image%2040.png)