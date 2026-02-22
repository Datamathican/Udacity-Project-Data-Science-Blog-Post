# StackOverflow Developer Data Analysis: What Drives a $100k Salary?

### Table of Contents
1. [Installation](#installation)
2. [Project Motivation](#project-motivation)
3. [File Descriptions](#file-descriptions)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing-authors-and-acknowledgements)

## Installation <a name="installation"></a>
The code was developed using Python 3.x in a Google Colab/Jupyter Notebook environment. The necessary libraries to run the notebook are:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`

No out-of-the-ordinary packages are required. To run the notebook, you will need to download the StackOverflow Developer Survey dataset (`survey_results_public.csv`) and place it in the same directory.

## Project Motivation<a name="project-motivation"></a>
For this Udacity Data Science Nanodegree project, I chose to analyze the StackOverflow Developer Survey to better understand the tech landscape and the factors that influence compensation. Specifically, I used the CRISP-DM process to answer:
1. How does years of professional coding experience relate to salary?
2. Does formal education level significantly impact earning a high salary?
3. Can we predict if a developer earns over $100k based on their background (experience, education, and organization size)?

## File Descriptions <a name="file-descriptions"></a>
* `StackOverflow_Analysis.ipynb`: A Jupyter Notebook containing all the code to gather, assess, clean, analyze, and model the data. It contains detailed comments and follows the CRISP-DM process.
* `README.md`: This file, detailing the project overview.
*(Note: The `survey_results_public.csv` file is not uploaded to this repository due to GitHub size constraints, but it can be downloaded directly from StackOverflow).*

## Results<a name="results"></a>
The main findings of the code can be found in the accompanying blog post available [(https://medium.com/@ima7600/the-100k-question-do-you-really-need-a-degree-to-make-bank-in-tech-403d8f5ff327?postPublishedType=repub)]. 

In short, the machine learning model revealed that years of professional coding experience heavily dictates whether a developer breaks the $100k threshold, vastly outweighing specific degrees. In a simulated prediction, a developer with 5 years of experience and a Master's degree at a large enterprise company had a near 0% probability of earning >$100k, proving that "time in seat" is the ultimate driver of high compensation in this dataset.

## Licensing, Authors, Acknowledgements<a name="licensing-authors-and-acknowledgements"></a>
Credit to [StackOverflow](https://insights.stackoverflow.com/survey) for providing the open-source dataset. Code is free to use.
