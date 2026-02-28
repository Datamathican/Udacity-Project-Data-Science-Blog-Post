# Udacity Data Science Nanodegree: Data Science Blog Post

## Project Overview
This project is part of the Udacity Data Science Nanodegree. For this project, I applied the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** methodology to analyze the Stack Overflow Developer Survey dataset. The goal of the project is to uncover insights about developer compensation and explore what background factors most strongly predict a six-figure salary in the tech industry.

### Business Questions
The analysis seeks to answer the following three key business questions:
1. How does the number of years of professional coding experience relate to salary?
2. Does formal education level significantly impact earning a high salary?
3. Can we accurately predict if a developer earns over $100k based on their background?

## Installation & Requirements
To run the code in this repository, you will need Python 3 installed along with the following data science libraries:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `jupyter`

You can install these dependencies using pip:
`pip install pandas numpy matplotlib seaborn scikit-learn jupyter`

## File Descriptions
* **`StackOverflow_Analysis-3.ipynb`**: The main Jupyter Notebook containing the end-to-end data analysis. It strictly follows the CRISP-DM framework (Business Understanding, Data Understanding, Data Preparation, Modeling, and Evaluation).
* **`README.md`**: This file, providing an overview of the project.
* **`survey_results_public.csv`**: The dataset used for this analysis (Note: depending on the year, this file might need to be downloaded directly from Stack Overflow if it exceeds GitHub's file size limits).

## Results & Findings
1. **Experience vs. Salary:** There is a clear positive correlation between years of coding experience and salary. The salary ceiling expands massively for developers who pass the 5-10 year mark in the industry.
2. **Education vs. Salary:** Formal education does play a role in average compensation. Globally, developers with Master's and Professional degrees average higher salaries compared to those with lower levels of formal education, though many self-taught developers still achieve high salaries.
3. **Predictive Modeling:** Using a Random Forest Classifier trained on features like age, education, remote work status, and years of experience, we were able to predict whether a developer earns over $100k with reasonable accuracy (approx. 67% weighted average), proving that these background traits are strong predictors of earning potential.

## Blog Post Publication
The full non-technical write-up of these findings has been published on Medium. 

**Read the blog post here:** [The $100k Question: Do You Really Need a Degree to Make Bank in Tech?](https://medium.com/@ima7600/the-100k-question-do-you-really-need-a-degree-to-make-bank-in-tech-403d8f5ff327)

## Acknowledgements
* Data provided by the annual [Stack Overflow Developer Survey](https://insights.stackoverflow.com/survey).
* Project architecture and rubric provided by the [Udacity Data Scientist Nanodegree Program](https://www.udacity.com/course/data-scientist-nanodegree--nd025).
