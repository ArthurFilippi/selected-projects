# Auditable prediction of the carbon intensity of a multi-market automotive portfolio

*Team research project, École Polytechnique, with a European banking partner.*

## Motivation

Measuring the carbon footprint of a vehicle-financing portfolio requires predicting the **carbon intensity** (gCO₂/km) of the financed vehicles, which is often missing from management databases. The paper builds an **auditable ML methodology** on a real, multi-country and heterogeneous dataset (seven markets, ≈ 800,000 observations):

- imputation of missing features (*fuzzy matching*), controlled by Jensen-Shannon and Wasserstein divergences;
- benchmark of four models (LightGBM, XGBoost, MLP) under cross-validation, with **SHAP** as a diagnostic tool;
- conformal prediction intervals (MAPIE);
- cross-market *dataset shift* analysis (domain classifier, PCA, AUC).

## Confidentiality

This work is subject to **confidentiality and intellectual property clauses** with the partner, who holds the IP on the code. It is a group project; I present **only my own contribution**, and in **reduced** form: **the code and the databases are confidential and are not part of this repository**, and operational considerations are omitted. The paper is limited to the scientific methodology. I would be happy to provide more details orally.

## References

For verification, my supervisors on the partner side are at BNP Paribas Personal Finance: **David Pomes** and **Christophe Bourdeaux**. Contact details on request.
