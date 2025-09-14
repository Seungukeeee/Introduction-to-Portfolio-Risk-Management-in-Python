# Portfolio composition and backtesting

Type: class
Course: Introduction to Portfolio Risk Management in Python (Introduction%20to%20Portfolio%20Risk%20Management%20in%20Pytho%2022ee0f71ffdc80e1b72bebdad253123f.md)
Done: Done

---

<aside>

ABOUT

- Portfolio composition and backtesting
</aside>

- you can think of portfolios as a bundle of individual stocks with different weights for each position.
    - The return of a portfolio is a linear combination of the weights and returns of each position. This assumes you’re using **discrete returns instead of log returns**.
    
    ![image.png](image%2016.png)
    
    ![image.png](image%2017.png)
    
    ** you can do it if you have an array of portfolio weights and a data frame of stock returns.
    
- Any good strategy should at least ideally outperform an equally weighted portfolio, which holds the same weight in every stock by default.

![image.png](image%2018.png)

![image.png](image%2019.png)

what you normally want to see is cumulative returns, or growth over time.

![image.png](image%2020.png)

- Market capitalization (시가총액)
    - it is the total value of all outstanding publicly traded shares of the company at any given time.
    - in order to calculate the market-cap weight of a given stock n, divide the market capitalization of that company by the sum of all the market capitalizations of all the stocks in your portfolio.
    
    ![image.png](image%2021.png)
    

### Storyline of the learning

## 📌 **Your Goal**

You want to build a **portfolio** — a basket of assets — that can help you **grow wealth** while managing **risk**. To do that, you need to make **strategic choices**, and then **evaluate** how well those choices would’ve worked in the real world.

But building a portfolio isn’t just picking stocks. It’s **designing a system** — a system where each part (asset, weight, return, time) interacts and creates **emergent behavior**.

---

## 🧱 **Stage 1: Portfolio Construction — “The Architecture”**

> “Before you simulate, you build. Before you build, you decide what matters.”
> 

### 🔹 Key Concepts Introduced:

| Concept | What It Means | Why It Matters |
| --- | --- | --- |
| **Assets** | Stocks, ETFs, bonds — your ingredients | Different assets behave differently. |
| **Weights** | How much of each asset you hold | Determines how much each asset affects your result. |
| **Market Capitalization** | Value of company = shares × price | Used in **cap-weighted** portfolios — the industry default. |
| **Equal-Weighting** | Every asset gets same importance | Removes bias from large companies. |
| **Portfolio Value** | Total worth of all your positions | Tracks how your strategy performs over time. |

### 🧩 How They Work Together:

You define **what to include (assets)** and **how much to allocate (weights)**. These weights are not arbitrary — they **reflect your beliefs**:

- Cap-weighted: “Let the market decide who matters.”
- Equal-weighted: “Give everyone a fair shot.”

This portfolio is not static — it moves with market prices. As prices shift, so does the portfolio’s value.

---

## 📈 **Stage 2: Portfolio Returns — “The Pulse”**

> “Now that you’ve built it, you need to understand how it breathes — how it changes, grows, or suffers.”
> 

### 🔹 Key Concepts Introduced:

| Concept | What It Means | Why It Matters |
| --- | --- | --- |
| **Returns** | % change in value over time | It’s what you gain or lose. |
| **Log Returns** | log(P_t / P_t-1) | Additive over time, better for modeling. |
| **Cumulative Return** | Compounded growth over time | Shows the power of consistency and time. |
| **Rolling Averages / Volatility** | How returns behave over windows | Capture trends and risks dynamically. |

### 🧩 How They Work Together:

Returns are **what the system produces**. Once your weights are in place, you calculate returns to see how well your strategy would’ve done over time.

Plotting **cumulative returns** shows the **narrative of growth** — peaks and valleys of your portfolio’s life.

---

## 🔬 **Stage 3: Backtesting — “The Time Machine”**

> “Now ask: what if I had done this 5 years ago? Would this portfolio have helped me? Or hurt me?”
> 

### 🔹 Key Concepts Introduced:

| Concept | What It Means | Why It Matters |
| --- | --- | --- |
| **Backtesting** | Applying your strategy to historical data | See if your logic holds up. |
| **Rebalancing** | Adjusting weights periodically | Keeps the portfolio aligned with strategy. |
| **Performance Metrics** | Sharpe Ratio, Max Drawdown, CAGR | Measure if the system was “good.” |

### 🧩 How They Work Together:

Backtesting puts your portfolio into **simulated history**. It helps you learn:

- Did it perform well overall (CAGR)?
- Was it too volatile (Standard Deviation)?
- Did it crash hard (Drawdown)?
- Was the return worth the risk (Sharpe)?

These metrics are your **system diagnostics**.

---

## 🔁 **Stage 4: Feedback & Refinement — “The Control Loop”**

> “The system is live. The market moves. What happens now?”
> 

Here’s where **interactions matter**:

- Your weights affect your risk.
- Market moves affect your asset values.
- Changes in volatility affect your Sharpe.
- Too much drawdown? Revisit allocation or diversification.
- Underperforming compared to a benchmark? Rethink your asset selection.

You may:

- **Change weights**: switch from cap to equal.
- **Add constraints**: “no more than 30% in tech.”
- **Try factor tilts**: prefer low-volatility or high-dividend assets.

The portfolio system is **iterative** — you run it, observe, and revise.

---

## 🕸️ **Putting It All Together — The Systemic Map**

```
[Asset Selection]
    ↓
[Weighting Scheme (Equal / Cap)]
    ↓
[Compute Portfolio Value over Time]
    ↓
[Calculate Returns & Risk Metrics]
    ↓
[Plot Cumulative Performance]
    ↓
[Backtest Strategy on Historical Data]
    ↓
[Evaluate Metrics: Sharpe, Drawdown, CAGR]
    ↓
[Refine Strategy: Rebalance, Reallocate]
    ↺ (feedback loop)

```

---

## 🎯 **Why It Matters in the Real World**

This process mirrors what real asset managers and quant analysts do daily:

- **Build portfolios** based on investment beliefs.
- **Test them** rigorously before investing.
- **Monitor them** and adapt as markets evolve.

You now see:

- Each concept isn’t isolated — it’s a **mechanism in a living engine**.
- Choices you make ripple through the system.
- You’re not just coding — you’re designing an **automated financial organism**.

---

## 🚦Closing Insight

> “To build a portfolio is to construct a hypothesis about the world. To backtest it is to confront that hypothesis with history. To iterate is to learn.”
>