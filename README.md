# Udacity Data Science Nanodegree: Data Science Blog Post

## Project Overview
This project is part of the Udacity Data Science Nanodegree. For this project, I applied the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** methodology to analyze the Stack Overflow Developer Survey dataset. The goal of the project is to uncover insights about developer compensation and explore what background factors most strongly predict a six-figure salary (`> $100k`) in the tech industry.

## Business Questions
The analysis seeks to answer the following three key business questions:
1. **Question 1:** How does the number of years of professional coding experience relate to salary?
2. **Question 2:** Does formal education level significantly impact earning a high salary?
3. **Question 3:** Can we accurately predict if a developer earns over $100k based on their background?

## Installation & Requirements
To run the code in this repository, you will need Python 3 installed along with the following data science libraries:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `jupyter`

You can install these dependencies using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```
## File Descriptions

StackOverflow_Analysis.ipynb: The main Jupyter Notebook containing the end-to-end data analysis. It strictly follows the CRISP-DM framework (Business Understanding, Data Understanding, Data Preparation & Missing Values Analysis, Modeling, Evaluation, and Deployment).

README.md: This file, providing an overview of the project, setup instructions, and key findings.
survey_results_public.csv: The dataset used for this analysis (Note: depending on the year, this file needs to be downloaded directly from the Stack Overflow Annual Developer Survey as it exceeds GitHub's file size limits).

## Results & Findings

Experience vs. Salary (Question 1): There is a clear positive correlation between years of coding experience and salary. Entry-level developers (0–3 years) cluster below the $100,000 mark, whereas the salary ceiling expands substantially for developers with 5–15 years of experience before plateauing at senior tenures (20+ years).

Education vs. Salary (Question 2): Formal education plays a noticeable role in average compensation. Globally, developers with Doctoral, Professional, and Master's degrees achieve higher average salaries compared to those with Associate degrees, some college study without a degree, or secondary school education.

Predictive Modeling (Question 3): Using a Random Forest Classifier trained on developer background features (Age, EdLevel, YearsCode, and OrgSize) across 23,947 cleaned records (using median imputation for numeric experience and mode imputation + One-Hot Encoding for categorical variables), the model predicts whether a developer earns over $100k with 67.6% accuracy (0.6759) (and a 0.66 weighted average F1-score) on the unseen test set.

## Blog Post Publication
The full non-technical write-up of these findings has been published on Medium. 

**Read the blog post here:** [The $100k Question: Do You Really Need a Degree to Make Bank in Tech?](https://medium.com/@ima7600/the-100k-question-do-you-really-need-a-degree-to-make-bank-in-tech-403d8f5ff327)

## Acknowledgements
* Data provided by the annual [Stack Overflow Developer Survey](https://insights.stackoverflow.com/survey).
* Project architecture and rubric provided by the [Udacity Data Scientist Nanodegree Program](https://www.udacity.com/course/data-scientist-nanodegree--nd025).
