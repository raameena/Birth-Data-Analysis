Skip to content
Navigation Menu
raameena
Birth-Data-Analysis

Type / to search
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
Settings
Unsaved changes
You have unsaved changes on this file that can be restored.
Birth-Data-Analysis
/
README.md
in
main

Edit

Preview
Indent mode

Spaces
Indent size

2
Line wrap mode

Soft wrap
Editing README.md file contents
Selection deleted


1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
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
  <a href="https://github.com/raameena/Birth-Data-Analysis/blob/main/Birth_Data_Analysis.Rmd">
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

Use Control + Shift + m to toggle the tab key moving focus. Alternatively, use esc then tab to move to the next interactive element on the page.
No file chosen
Attach files by dragging & dropping, selecting or pasting them.
