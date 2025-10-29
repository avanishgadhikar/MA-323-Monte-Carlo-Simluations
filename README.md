# 📚 MA 323: Monte Carlo Simulation Lab Course (IITG, 2024)

This repository contains the **implementations, reports, and simulations** developed as part of the **MA 323: Monte Carlo Simulation Laboratory** course at IIT Guwahati (2024).  
The assignments explore fundamental and advanced techniques in **random number generation**, **variance reduction**, and **stochastic process modeling**, culminating in the simulation of complex financial and probabilistic systems.

---

## ⚙️ Core Topics & Techniques

The course was structured around **three main pillars** of Monte Carlo methods, progressing from basic random number generation to advanced stochastic modeling and quasi-Monte Carlo analysis.

---

### 🧩 I. Random Number Generation and Sampling (Labs 01–05)

This module established the foundation for random number theory and sampling techniques.

| Topic | Description |
|--------|-------------|
| **Pseudo-Random Numbers** | Analysis of the **Linear Congruence Generator (LCG)** — including period length, uniformity, and the lattice structure observed in 2D plots. |
| **Inverse Transform Method** | Generated samples from continuous PDFs such as f(x) = 3(1 − x)² and from piecewise-defined distributions. Compared **Empirical CDFs** with theoretical CDFs. |
| **Acceptance–Rejection (A–R)** | Implemented A–R for complex distributions such as f(x) = 20x(1 − x)³ and f(x) ∝ x^(α−1) * e^(−x) for 0 < x < 1. Analyzed **rejection constants** and **efficiency**. |
| **Normal Variate Generation** | Compared **Box–Muller** and **Marsaglia–Bray** methods for generating N(0,1) samples — focusing on runtime and rejection ratio performance. |
| **Multivariate Sampling** | Simulated samples from a **Bivariate Normal Distribution** N₂(μ, Σ) for varying correlation parameters and visualized their scatter structure. |

---

### 📉 II. Variance Reduction & Estimation (Labs 06–08)

This module focused on improving the **accuracy and efficiency** of Monte Carlo estimators (IM).

| Technique | Description |
|------------|-------------|
| **Crude Monte Carlo** | Estimated expectations such as I = E[e^(√U)] and I = E[e^U]. Computed **95% confidence intervals** for the sample mean estimator. |
| **Antithetic Variables** | Implemented the estimator  **ÎM = (1/M) Σ [(exp(√Ui) + exp(√(1 − Ui))) / 2]**. Compared **variance** and **confidence interval width** with the crude estimator. |
| **Control Variates** | Applied the **Control Variate** method using U as the control variable to reduce variance in the estimate (ÎM). |
| **Advanced Variance Reduction** | Applied **Conditioning** and **Stratification** to estimate probabilities in a **Compound Poisson model**, demonstrating improved precision and reduced estimator variance. |

---

### 📈 III. Stochastic Processes & Quasi-Monte Carlo (Labs 09–11)

This final module focused on **modeling continuous-time stochastic processes** and exploring **quasi-random sampling** techniques.

| Topic | Description |
|--------|-------------|
| **Brownian Motion (BM)** | Simulated **Standard Brownian Motion** and BM(μ, σ²) using discrete-time recursion. Extended to models with time-dependent drift and volatility. |
| **Geometric Brownian Motion (GBM)** | Modeled financial asset prices using **GBM**. Estimated parameters μ and σ from real stock price data and analyzed the convergence of E[S(T)]. |
| **Jump Diffusion Process** | Simulated the process X(t) = (Wiener component) + (Poisson jump component) to capture non-continuous price movements. Studied the effect of **jump intensity (λ)** on dynamics. |
| **Quasi–Monte Carlo (QMC)** | Analyzed the **limitations of LCGs** by computing **discrepancy**. Implemented and visualized **Low-Discrepancy Sequences (LDS)** (e.g., Sobol, Halton) versus pseudo-random numbers to demonstrate superior uniformity. |

---

## 📖 References & Resources

- **Glasserman, P. (2004).** *Monte Carlo Methods in Financial Engineering.* Springer.  
  *Cited in Lab 09 and Lab 10.*

- **Seydel, U. (2012).** *Tools for Computational Finance (5th Edition).* Springer.  
  *Used as supplementary background material.*

---

🧮 *End of README*
