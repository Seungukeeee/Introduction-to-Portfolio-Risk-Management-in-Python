# Risk modeling techniques

Type: class
Course: Credit Risk Modeling in Python (Credit%20Risk%20Modeling%20in%20Python%20228e0f71ffdc80b7bc79e2d13be31878.md)
Done: Done

---

<aside>

ABOUT

- Risk modeling techniques
</aside>

- Discrete-time hazard model (point in time): the probability of default is a point-in-time event. This means all of the training data and the predictions are set for a specific point in time.
- The framework used is known as a structural model framework meaning that the training data was used to explain the probability of default.
- Other techniques
    - Through-the-cycle model (continuous time): macro-economic conditions and other effects are used, but the risk is seen as an independent event.
    - Reduced-form model framework: a statistical approach estimating probability of default as an independent Poisson-based event.
- Choosing models
    - many financial sectors prefer model interpretability: Complex or “black-box” models are a risk because the business cannot explain their decisions fully.
    - Deep neural networks are often **too complex**.