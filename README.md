# Differential Privacy and Cooperation in Public Goods Games

> **A Game-Theoretic Analysis using Differential Privacy**

<p align="center">
  <img src="images/Linkedin Infographic.png" alt="Project Infographic" width="950">
</p>

---

## Overview

This repository contains the report and visual summary of my bachelor's project exploring the relationship between **Differential Privacy** and **strategic cooperation** in repeated **Public Goods Games (PGGs)**.

While Differential Privacy is primarily designed to protect sensitive information, this project investigates a different question:

> **Can introducing controlled uncertainty actually encourage cooperation?**

To study this, I modeled a repeated Public Goods Game in which players observe **noisy aggregate feedback** generated using the **Laplace mechanism** of Differential Privacy. Instead of reacting to perfect information, agents update their beliefs using Bayesian inference before making future decisions.

The project studies how different privacy levels influence:

* Cooperation
* Strategic behaviour
* Social welfare

---

## Motivation

Repeated Public Goods Games often suffer from the **free-rider problem**.

With perfect information, even small deviations from cooperation can trigger retaliation, eventually causing cooperation to collapse.

Introducing Differential Privacy changes the information structure of the game. Rather than observing exact public contributions, players receive noisy feedback and must reason under uncertainty.

This raises an interesting question:

> **Can privacy serve not only as a data protection mechanism, but also as a mechanism for improving strategic outcomes?**

---

## Methodology

The project follows the workflow below.

```text
Repeated Public Goods Game
          │
          ▼
Differential Privacy
(Laplace Mechanism)
          │
          ▼
Noisy Aggregate Feedback
          │
          ▼
Bayesian Belief Updating
          │
          ▼
Multi-Agent Simulation
          │
          ▼
Cooperation & Social Welfare Analysis
```

---

## Key Findings

The simulations reveal a clear trade-off between privacy and coordination.

| Privacy Level                   | Observation                                                                                                 |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Very High Privacy (Small ε)** | Excessive noise makes coordination difficult and reduces cooperation.                                       |
| **Very Low Privacy (Large ε)**  | Players detect every deviation and tend to overreact, destabilizing cooperation.                            |
| **Moderate Privacy**            | Balances uncertainty and information, resulting in the highest cooperation and near-optimal social welfare. |

The central takeaway is:

> **Privacy is not only a tool for protecting information—it can also influence incentives and shape strategic behaviour.**

---

## Concepts Explored

* Game Theory
* Public Goods Game
* Differential Privacy
* Laplace Mechanism
* Bayesian Belief Updating
* Multi-Agent Simulation
* Social Welfare Analysis

---

## Results

### Cooperation vs Privacy Level

<p align="center">
  <img src="figures/Cooperation vs Privacy.png" width="700" alt="Cooperation vs Privacy">
</p>

As privacy increases from extremely low levels, cooperation improves because agents become less likely to overreact to small fluctuations. However, excessive privacy introduces too much uncertainty, making coordination difficult. The results suggest that **moderate privacy provides the best trade-off** between information quality and behavioural stability.

---

### Social Welfare vs Privacy Level

<p align="center">
  <img src="figures/Welfare vs Privacy.png" width="700" alt="Welfare vs Privacy">
</p>

Social welfare follows a similar pattern. Moderate privacy maintains enough information for coordination while preventing unnecessary retaliation, resulting in near-optimal collective outcomes.

---

## Project Report

The complete project report contains:

* Mathematical formulation of the model
* Game-theoretic analysis
* Differential Privacy framework
* Bayesian belief updating
* Simulation methodology
* Python implementation
* Experimental results
* Discussion and conclusions

📄 **report.pdf**

---

## Repository Contents

```text
.
├── README.md
├── report.pdf
├── LICENSE
│
├── images/
│   └── Linkedin Infographic.png
│
└── figures/
    ├── Cooperation vs Privacy.png
    └── Welfare vs Privacy.png
```

---

## Future Directions

Some natural extensions of this work include:

* Bayesian Nash Equilibrium analysis
* Reinforcement Learning agents
* Federated Learning applications
* Alternative Differential Privacy mechanisms
* Heterogeneous agent populations
* Mechanism design for decentralized systems

---

## Author

**Dhruv Verma**

Bachelor's Project

If you have suggestions, feedback, or ideas for extending this work, feel free to connect with me on LinkedIn or open an issue in this repository.

---

## License

This project is licensed under the MIT License.

