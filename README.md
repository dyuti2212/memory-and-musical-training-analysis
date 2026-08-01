# 🎵 Memory and Musical Training Analysis

## About the Project

Have you ever wondered if learning music actually improves your memory?

This project explores that question using real-world cognitive psychology data and machine learning. Specifically, it investigates whether people with greater musical experience perform better on different types of working memory tasks.

Rather than asking *"Does music make you smarter?"*, the project asks a more focused question:

> **Is musical experience associated with all forms of working memory, or is the relationship stronger for auditory memory?**

To answer this, I analyzed data from over **1,400 participants** using exploratory data analysis, feature engineering, and predictive machine learning models.

---

## Objectives

The main goals of this project were to:

- Explore the relationship between musical experience and working memory.
- Compare three different memory domains:
  - 🎼 Melody Span (Auditory Working Memory)
  - 🔢 Digit Span (Verbal Working Memory)
  - 🧩 Spatial Span (Visuospatial Working Memory)
- Build machine learning models to predict memory performance.
- Compare a simple interpretable model (Linear Regression) with a more complex model (Random Forest Regression).

---

## Project Workflow

```text
Raw Dataset
      │
      ▼
Data Cleaning & Quality Assessment
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Feature Engineering & Selection
      │
      ▼
Linear Regression
      │
      ▼
Random Forest Regression
      │
      ▼
Model Comparison & Conclusions
```

## Dataset

The dataset contains cognitive test scores and questionnaire responses from more than **1,400 participants**.

Some of the variables include:

- Age
- Years of Education
- Socioeconomic Status
- Musical Training (Gold-MSI)
- Musical Sophistication
- Active Musical Engagement
- Big Five Personality Traits

The target variables are:

- Melody Span
- Digit Span
- Spatial Span

---

## Models Used

### Linear Regression

Linear Regression was used as the primary model because it is simple, interpretable, and well suited for understanding how different variables relate to memory performance.

### Random Forest Regression

Random Forest was implemented as a comparison model to determine whether a more complex nonlinear algorithm could improve prediction accuracy.

---

## Results

### Linear Regression

| Memory Task | MAE | RMSE | R² |
|-------------|----:|-----:|----:|
| Melody Span | **4.33** | **5.61** | **0.248** |
| Digit Span | **1.83** | **2.24** | **-0.006** |
| Spatial Span | **1.42** | **2.04** | **0.026** |

### Linear Regression vs Random Forest

| Model | MAE | RMSE | R² |
|--------|----:|-----:|----:|
| Linear Regression | **4.33** | **5.61** | **0.248** |
| Random Forest | **4.45** | **5.68** | **0.230** |

Interestingly, the simpler Linear Regression model slightly outperformed Random Forest, suggesting that the relationships in this dataset are mostly linear.

---

## Key Findings

Some of the most interesting findings from the analysis were:

- Musical experience was a strong predictor of **Melody Span** performance.
- The same predictors explained almost none of the variation in **Digit Span**.
- Musical experience had only a weak relationship with **Spatial Span**.
- Gold-MSI General Sophistication and Musical Training consistently emerged as the most important predictors.
- A simpler Linear Regression model performed slightly better than Random Forest while remaining much easier to interpret.

Overall, the results suggest that musical experience is more strongly associated with **auditory working memory** than with verbal or visuospatial working memory.

---

## Limitations

Like any data analysis project, this study has a few limitations:

- The dataset is observational, so the results show **associations rather than causation**.
- The models explain only part of the variability in memory performance.
- Musical experience was measured using self-reported questionnaire scores.
- Other cognitive or environmental factors that may influence memory were not included in the dataset.

---

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## What I Learned

This project gave me hands-on experience with the complete machine learning workflow—from data cleaning and exploratory analysis to feature engineering, model building, evaluation, and interpretation.

One of the biggest takeaways was that **a more complex model isn't always a better model**. In this case, Linear Regression not only performed slightly better than Random Forest but also provided much clearer insights into the relationship between musical experience and memory.

---

## Author

**Dyuti**

B.Tech Student | Aspiring Data Scientist

I'm interested in Machine Learning, Data Science, and using data-driven approaches to understand human behavior and cognition.