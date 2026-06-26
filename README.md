````markdown
# Differential Privacy and Cooperation in Public Goods Games

<p align="center">
  <img src="images/infographic.png" width="900" alt="Project Infographic">
</p>

<p align="center">
  <strong>A Game-Theoretic Analysis using Differential Privacy</strong>
</p>

---

## Overview

This project explores how **Differential Privacy (DP)** influences strategic behaviour in the **Public Goods Game (PGG)**, a classical model used to study cooperation and the free-rider problem.

Instead of revealing the exact number of contributors after each round, the model introduces **Laplace noise** through Differential Privacy. Players then use **Bayesian belief updates** to infer the true level of cooperation before deciding their next action.

The objective is to understand how different privacy levels affect:

- Cooperation
- Strategic behaviour
- Social welfare

---

## Motivation

Differential Privacy is generally viewed as a technique for protecting sensitive information.

This project explores a different question:

> **Can privacy itself influence strategic behaviour?**

In repeated Public Goods Games, perfectly transparent systems allow players to immediately detect defections, often triggering retaliation and eventually leading to the collapse of cooperation.

Introducing controlled uncertainty changes the information available to players, creating an interesting trade-off between privacy and coordination.

---

## Methodology

The simulation follows the pipeline below:

```text
Repeated Public Goods Game
          ↓
 Differential Privacy
 (Laplace Mechanism)
          ↓
 Noisy Feedback
          ↓
 Bayesian Belief Updates
          ↓
 Multi-Agent Simulation
          ↓
 Cooperation & Welfare Analysis
````

---

## Key Findings

The simulations reveal an interesting trade-off.

| Privacy Level                   | Behaviour                                                                                      |
| ------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Very High Privacy (Small ε)** | Signals become unreliable, making coordination difficult.                                      |
| **Very Low Privacy (Large ε)**  | Players detect every deviation and tend to overreact.                                          |
| **Moderate Privacy**            | Balances uncertainty and information, resulting in the highest cooperation and social welfare. |

One of the main insights from this project is that **privacy is not only a tool for protecting data—it can also influence incentives and strategic behaviour.**

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Differential Privacy (Laplace Mechanism)
* Bayesian Belief Updating
* Game Theory
* Multi-Agent Simulation

---

## Repository Structure

```text
.
├── README.md
├── report.pdf
├── simulation.py
├── requirements.txt
├── images/
│   └── infographic.png
├── figures/
│   ├── cooperation_vs_privacy.png
│   └── welfare_vs_privacy.png
└── LICENSE
```

---

## Results

### Cooperation vs Privacy Level

<p align="center">
  <img src="figures/cooperation_vs_privacy.png" width="650">
</p>

As privacy increases from extremely low levels, cooperation improves because agents no longer overreact to small fluctuations.

However, excessive privacy introduces too much uncertainty, making coordination difficult.

This suggests that **moderate privacy levels provide the best trade-off**.

---

### Social Welfare vs Privacy Level

<p align="center">
  <img src="figures/welfare_vs_privacy.png" width="650">
</p>

Social welfare follows a similar trend.

Moderate privacy maintains enough information for coordination while preventing unnecessary retaliation, leading to near-optimal welfare.

---

## Future Improvements

Some possible extensions include:

* Bayesian Nash Equilibrium analysis
* Quantal Response Equilibrium
* Reinforcement Learning based agents
* Heterogeneous agent populations
* Alternative Differential Privacy mechanisms
* Federated Learning applications
* Larger-scale simulations

---

## Author

**Dhruv Verma**

Bachelor's Project

If you have suggestions or ideas for extending this work, feel free to open an issue or connect with me on LinkedIn.

##

```
```
