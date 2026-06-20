
# Final Project

## Research Topic: The Joint Effects of Biological Sex and Exercise Habits on Body Weight

🎥 **Project Oral Presentation Video Link**: (https://youtu.be/ZVCe3tIpDnU)

---

## Project Overview

This repository contains the complete data processing pipeline, statistical analysis results, and visualization summaries for this research project. The objective of this study is to investigate how biological sex (a physiological variable) and lifestyle choices (exercise habits) jointly interact to influence an individual's body weight.

---

## 1. Research Questions and Variable Definitions

### Research Questions

* **Phase I: Baseline Gap (Inherent Differences)** — Does biological sex alone generate a major, statistically significant baseline difference in individual body weight when lifestyle habits are completely excluded?
* **Phase II: Exercise Intervention & Interaction Matrix** — How does exercise affect the body weight of males and females respectively when introduced into the model? Furthermore, when biological sex and exercise habits are combined, do they create an interdependent interference pattern (Interaction Effect) on body weight?

### Variable Definitions

* **Independent Variable 1 (Sex_Gender)**: Categorical Variable [Male, Female]
* **Independent Variable 2 (Exercise_Habit)**: Categorical Variable [High (Regularly Exercises), Low (Rarely Exercises)]
* **Dependent Variable (Body_Weight_KG)**: Continuous Numerical Variable [Body weight data in kilograms (KG)]

---

## 2. Data Processing and Statistical Methodology

### Data Cleaning and Preprocessing

* **Filtering and Integrity**: Core analytical fields including sex, exercise habits, and body weight were precisely isolated. All rows containing missing values (NaN) were dropped to ensure data authenticity and complete integrity.
* **Variable Recoding**: Original categorical codes were transformed and standardized into clear English labels ("Male", "Female", "High", and "Low").
* **Sample Dimensions**: This project utilizes a strictly balanced design with a total sample size of **N = 1,000** observations (exactly 250 observations per cross-sectional group) to eliminate any statistical power bias caused by unequal group sizes.

### Statistical Analysis Pipeline

1. **Two-Way Analysis of Variance (Two-Way ANOVA)**: Conducted on the full dataset to evaluate the main effects of biological sex, exercise habits, and the significance of their interaction effect on overall body weight.
2. **Simple Main Effects**: As an advanced decomposition step, the dataset was stratified by sex to horizontally contrast and isolate the precise impact and strength of exercise habits within the "Male cohort" and the "Female cohort" independently.

---

## 3. Core Statistical Results

### Descriptive Statistics Summary

* **Female / High Exercise**: Mean Weight = 61.6585 kg | Standard Deviation (SD) = 3.3537
* **Female / Low Exercise**: Mean Weight = 63.5307 kg | Standard Deviation (SD) = 3.9576
* **Male / High Exercise**: Mean Weight = 72.2724 kg | Standard Deviation (SD) = 4.4913
* **Male / Low Exercise**: Mean Weight = 76.4879 kg | Standard Deviation (SD) = 4.8303

### Simple Main Effects Cross-Gender Contrast ANOVA Table

| Subgroup / Source | df | Mean Square | F | Sig. (p-value) |
| --- | --- | --- | --- | --- |
| **Exercise Effect within Male** | 1.0 | 2221.3654 | 102.1178 | 5.7911e-22 |
| *Error within Male (Residual)* | 498.0 | 21.7529 | NaN | NaN |
| **Exercise Effect within Female** | 1.0 | 438.0772 | 32.5634 | 1.9826e-08 |
| *Error within Female (Residual)* | 498.0 | 13.4530 | NaN | NaN |

---

## 4. Data Interpretation and Insights

### Phase I: Macro Baseline Divergence (Inherent Differences Only)

Biological sex exerts a massive, overriding baseline influence on human body weight. In our initial macro-level comparison (completely excluding exercise habits), the baseline mean weight for the male cohort is naturally and significantly higher than that of the female cohort.

### Phase II: Stratified Deep-Dive (Factoring in Exercise)

* **Insights within the Male Cohort**: Having an exercise habit makes an extraordinary difference for men. Males with a regular exercise routine have an average body weight that is **4.22 kg** lighter than sedentary males (F = 102.12, p < 0.001).
* **Insights within the Female Cohort**: Exercise is also highly effective for women. Females with a regular exercise routine are, on average, **1.87 kg** lighter than sedentary females (F = 32.56, p < 0.001).

### Core Conclusion: Why Do They Cross-Interfere?

While regular, structured exercise successfully correlates with a lower body weight across both genders, the weight gap between active and sedentary individuals is vastly wider for men (**4.22 kg** reduction) than it is for women (**1.87 kg** reduction).

Because exercise demonstrates a much more aggressive and potent impact on male body mass compared to female body mass, this mathematically proves a highly significant **Interaction Effect** (p = 1.1188e-05). In short, biological sex and lifestyle habits do not operate in isolation; they cross-interfere and compound to scale final body weight outcomes.
