# Option hedging in the Black-Scholes model

*Applied mathematics project, École Polytechnique (CMAP). Joint work with **Vincent Neves**.*

## Topic

Construction of a **hedging portfolio** for an option under a discretised Black-Scholes model, and study of the convergence of the replication error, in three stages:

1. **Theory**: risk-neutral measure, **Black-Scholes formula**, call-put parity, and the price as the solution of a **PDE**.
2. **Discrete hedging**: *delta* strategy; error $\Delta_T^h = V_T^h - \Phi(S_T)$ (empirically $\mathbb{E}[|\Delta_T^h|]\propto N^{-1/3}$); estimation of the *delta* by **Monte Carlo**; discontinuous **digital** *payoff* (adaptive resampling near maturity).
3. **Market data**: consistent volatility estimator, applied to the **DAX**.

## Contents

- `hedging_black_scholes.ipynb`: full notebook (proofs + code + figures).
- `DAX.csv`: closing prices used for the calibration.

```bash
pip install numpy scipy matplotlib pandas yfinance
jupyter lab hedging_black_scholes.ipynb
```

> The text of the notebook is in English. The figures were produced by the original run and their axis labels are still in French.
