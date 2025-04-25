# Modeling the Impact of Student Habits on Academic Performance

This project explores how students' daily habits — such as study time, sleep, screen time, and mental health — influence academic performance. Using a dataset of 1,000 students, we built and evaluated predictive models to estimate exam scores based on lifestyle factors.

---

## Dataset

The dataset used is `student_habits_performance.csv`, which includes:

- Study hours, sleep duration, screen time
- Diet quality, exercise frequency, mental health rating
- Academic performance (final exam score)

---

## Preprocessing Steps

- Handled missing values (`parental_education_level`)
- Encoded categorical variables (binary, ordinal, one-hot)
- Dropped irrelevant columns (`student_id`)
- Scaled numerical features for modeling

---

## Exploratory Data Analysis

- Histograms to explore distributions and spot outliers
- Correlation matrix to evaluate relationships between behaviors and scores
- Key finding: **Study time** had a strong positive impact; **social media** had a moderate negative impact

---

## Modeling & Results

We tested two models:

| Model              | RMSE  | R² Score |
|-------------------|-------|----------|
| Linear Regression | 5.09  | 0.90     |
| Random Forest     | 6.25  | 0.85     |

**Linear Regression** performed better overall and was chosen as the final model.

---

## Key Insights

- Students who study more tend to perform significantly better.
- Excessive screen time (social media and Netflix) negatively impacts exam scores.
- Sleep and mental health had small positive effects.

---

## Conclusion

This project shows how student habits can be used not only to understand performance but also to predict it. The findings may help students and educators focus on actionable behavior changes.
These findings give us concrete levers for improvement. For instance, reducing social media use by 1 standard deviation could yield nearly half the benefit of increasing study time by the same amount - a more achievable behavioral change for many students.
While these results are compelling, we should view them as indicating associations rather than proven causal relationships. Future work could incorporate experimental designs to strengthen our conclusions.

---

## Tools Used

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Google Colab  
