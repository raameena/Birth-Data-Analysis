# Birth-Data-Analysis

Over the course of one month, myself and two others gathered data from [Kaggle](https://www.kaggle.com/datasets/danbraswell/temporary-us-births/code) to determine conclusions for **two essential questions:**

1. How does maternal educational attainment influence birth outcomes, such as birth weight and maternal age, across different states and years in the U.S.?

2. Are mothers with lower levels of education more likely to have multiple children compared to those with higher educational attainment?


## Functions and Methods

1. **Data Cleaning and Preparation:**

Used dplyr and tidyverse functions like mutate(), as_tibble(), and na.omit() to transform variable types, handle missing values, and prepare the dataset for analysis.

2. **Descriptive and Inferential Statistics:**

Calculated summary statistics with group_by() and summarise() to explore trends by education level. Applied ANOVA (aov) and linear regression (lm) to test the effects of maternal education and age on birth weight, including interaction effects.

3. **Data Visualization:**

Employed ggplot2 to create various plots, such as bar charts, scatterplots, violin plots, and line graphs, illustrating relationships across states and education levels. Used facet_wrap() to compare across multiple states and geom_text_repel() for labeling clarity.

4. **Classification and Modeling:**

Built a logistic regression model using glm() to classify whether a mother had a higher education level based on her age and her child’s birth weight. This allowed prediction and evaluation of how demographic factors relate to educational attainment.


## Conclusions

1. **Maternal education is inversely related to fertility rates:** Women with high school or some college education have more children, while those with advanced degrees tend to delay childbirth and have fewer births overall.

2. **Higher education correlates with better birth outcomes:** Educated mothers are more likely to have healthier babies, likely due to improved prenatal care access, health knowledge, and economic resources.

3. **Geographic disparities reflect educational and reproductive trends:** Northeastern and Western states show more college-educated mothers and later childbearing compared to the South, indicating regional inequality in maternal resources and planning.

4. **Policy implications point to education as a lever for better outcomes:** The findings support targeting interventions by region and education level, and call for further study into related factors like paternal education and local support systems.
