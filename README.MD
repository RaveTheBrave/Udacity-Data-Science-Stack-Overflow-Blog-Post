# How AI Is Shaping Developers' Work and Careers

## Project Overview

Artificial intelligence tools are becoming increasingly common in software development. Developers use AI to assist with coding, troubleshooting, learning new technologies, and completing repetitive tasks.

This project analyzes responses from the Stack Overflow Developer Survey to explore how AI adoption relates to developers' careers.

The analysis focuses on three main questions:

1. How does AI adoption vary across different career stages?
2. Is AI usage associated with differences in developer salary?
3. How does AI usage relate to developers' views about AI threatening their current jobs?

A machine learning classification model was also developed to explore whether developer characteristics can help predict AI adoption.

## Libraries Used

The analysis was completed in Python using the following libraries:

- **pandas** – data loading, cleaning, manipulation, and analysis
- **NumPy** – numerical operations
- **Matplotlib** – data visualization
- **SciPy** – statistical testing
- **scikit-learn** – preprocessing, logistic regression, model evaluation, and feature importance

## Repository Files

- **`Stack Overflow Blog Post.ipynb`** – Jupyter Notebook containing the complete data cleaning, exploratory analysis, statistical testing, modeling, evaluation, and visualizations.
- **`results.csv`** – Stack Overflow Developer Survey dataset used for the analysis.
- **`index.md`** – Blog post summarizing the major findings for a non-technical audience.
- **`images/`** – Images and charts used by the GitHub Pages blog post.
- **`README.md`** – Overview and documentation for the project.

## Summary of Results

### Career Stage and AI Adoption

AI adoption was common across all career stages but generally declined as professional experience increased.

Approximately:

- **83.1%** of early-career developers used AI tools.
- **81.9%** of mid-career developers used AI tools.
- **79.2%** of experienced developers used AI tools.
- **71.4%** of highly experienced developers used AI tools.

The relationship between career stage and AI adoption was statistically significant, although the strength of the relationship was relatively small.

### AI Usage and Developer Salary

AI users did not have higher salaries overall.

The median annual compensation was approximately:

- **$74,772 for AI users**
- **$80,871 for non-AI users**

Although the salary distributions were statistically different, the effect size was very small. This suggests that AI usage alone has little relationship with developer compensation.

### AI Usage and Career Outlook

AI users were slightly more likely to report that AI threatens their current job.

Approximately:

- **15.2% of AI users** viewed AI as a threat to their job.
- **11.2% of non-AI users** viewed AI as a threat.

Most respondents in both groups did not consider AI a threat to their current employment. The relationship was statistically significant but very weak.

### Predicting AI Adoption

A balanced logistic regression model was created to predict whether a respondent was an AI user.

The model achieved:

- **63.5% balanced accuracy**
- **0.689 ROC-AUC**

Developer role was the most important predictor in the model, followed by country and years of coding experience.

Overall, the model showed that developer characteristics contain some information about AI adoption, but they are not sufficient to predict an individual's AI usage with high accuracy.

## Acknowledgments

The dataset used in this project comes from the **Stack Overflow Developer Survey**.

This project was completed as part of the **Udacity Data Science Nanodegree** program.

Thanks to Stack Overflow for making the survey data available for analysis.
