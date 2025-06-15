<!-- ---------------------------------------------------------
  Birth-Data-Analysis · Maternal Education & Birth Outcomes
---------------------------------------------------------- -->

<h1 align="center">📊 Birth-Data-Analysis</h1>

<p align="center">
  <a href="https://raameena.github.io/Portfolio/posts/BirthDataAnalysis_Post/">
    <img src="https://img.shields.io/badge/demo-live%20post-2ea44f?logo=githubpages&logoColor=white" alt="Live demo badge">
  </a>
  <a href="https://www.kaggle.com/datasets/danbraswell/temporary-us-births">
    <img src="https://img.shields.io/badge/dataset-Kaggle-blue?logo=kaggle" alt="Kaggle badge">
  </a>
  <a href="[https://github.com/raameena/Birth-Data-Analysis/blob/main/Birth_Data_Analysis.Rmd](https://github.com/raameena/Birth-Data-Analysis/blob/main/Research_Births.Rmd)">
    <img src="https://img.shields.io/badge/code-R%20Markdown-75AADB?logo=r" alt="R Markdown badge">
  </a>
</p>

---

### ♡ Project Overview
In one month, a three-person team and I analysed **3.1 M U.S. birth records (2016-2021)** to answer two guiding questions:

1. **How does maternal education affect birth outcomes**—birth weight, maternal age—across states and years?
2. **Do mothers with lower education levels have more children** than those with higher education?

The full write-up is published on my portfolio 👉 **[read it here](https://raameena.github.io/Portfolio/posts/BirthDataAnalysis_Post/).**

---

## ♡ Methods & Workflow

| Stage | Tools / Functions |
|-------|-------------------|
| **Data prep** | `dplyr::mutate`, `as_tibble`, `na.omit` |
| **Descriptive stats** | `group_by` + `summarise` |
| **Inferential stats** | `aov` (one-way ANOVA), `lm` (linear regression), interaction terms |
| **Classification** | `glm(family = binomial)` — logistic model predicting **education level ↔︎ mother’s age & birth weight** |
| **Visualisation** | `ggplot2` (`geom_violin`, `facet_wrap`, `geom_text_repel`) |

---

## ♡ Key Findings

| # | Insight |
|---|---------|
| **1. Fertility vs. education** | Mothers with only a high-school diploma averaged **0.8 more children** than those with advanced degrees. |
| **2. Healthier babies** | Each additional education tier correlated with a **+105 g increase in mean birth weight** (p < 0.01). |
| **3. Regional disparities** | Northeast & West show later child-bearing and higher degrees; the South lags behind. |
| **4. Policy lever** | Investing in women’s education may simultaneously reduce high-risk births and unplanned fertility. |

---

## ♡ Repo Structure

```text
.
├─ Birth_Data_Analysis.Rmd   # reproducible analysis notebook
├─ /data/                    # raw & cleaned CSVs
├─ /figures/                 # ggplot outputs
└─ /docs/                    # knitted HTML report (optional GitHub Pages)
