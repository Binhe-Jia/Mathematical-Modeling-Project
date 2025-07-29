# Mathematical Modeling Project: Rent and Population Dynamics in Oronto

This project models the dynamic interaction between housing rent and population size in a hypothetical city called **Oronto**. Conducted for MAT244 (Differential Equations) at the University of Toronto, the project proposes mathematical solutions to address rising rent and population decline through policy-based interventions.

##  Objective

> How can a city government stabilize rent prices and prevent population outflow using policy tools?

We explore how rent control—based on real-time population trends—can help stabilize both rent and population over a 50-year horizon, using systems of differential equations.

##  Model Overview

We began with an existing model (provided by the fictional Housing Institute of Greater Oronto, HIGO):

- **Original HIGO Model:**
  - Models population growth as a logistic function with rent as a deterrent.
  - Assumes rent grows exponentially due to inflation.
  - **Limitation:** Rent and population are decoupled, leading to uncontrolled rent spikes and population collapse.

- **Proposed Modified Model:**
  - Retains the original population equation:
    ```
    P′(t) = P(t) · (10 − P(t)) − R(t)
    ```
  - Introduces a revised rent equation that responds to population changes:
    ```
    R′(t) = 0.5 · R(t) − 0.5 · P′(t)
    ```
  - **Interpretation**: Rent growth is reduced when population increases and allowed to rise when population falls.

##  Key Results

- **Rent Stabilization**: The modified model predicts that rent decreases in the first few years and then grows steadily—unlike the uncontrolled exponential growth in the HIGO model.
- **Population Retention**: The mass outflow of population observed in the original model is eliminated.
- **Budget Feasibility**: Total required government subsidy over 50 years is **$18.46 billion**, or about **$36.92 per resident annually**—a feasible cost for a city of 10 million.
- **Policy Insight**: Monthly rent subsidies based on population trends can yield long-term stability with moderate fiscal effort.

##  Tools Used

- Simulations and numerical approximations done via:
  - Euler’s method
  - Desmos (visual phase portraits and component graphs)


##  Authors

- **Eric Lu**
- **Binhe Jia**

##  Assumptions & Constraints

- The government can **only** influence rent (not directly control population).
- The model is intended for **medium-term planning (≤50 years)**.
- Population is capped at **10 million**.
- Inflation rate is fixed; real-world macroeconomic shifts are not modeled.

##  Citation

This project was submitted in November 2024 for MAT244: Introduction to Ordinary Differential Equations at the University of Toronto.

---
