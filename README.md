
# What Factors Determine Income? (Adult Census Dataset)

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![FASTAI](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Scikit-Learn](https://img.shields.io/badge/ML-Scikit--Learn-yellow)
![XGBoost](https://img.shields.io/badge/Model-XGBoost-red)
![LightGBM](https://img.shields.io/badge/Model-LightGBM-success)
![CatBoost](https://img.shields.io/badge/Model-CatBoost-orange)
![Optuna](https://img.shields.io/badge/Tuning-Optuna-blueviolet)

School project realized by Bonifas Olivier, Filloux Louis, and Gendronneau Maël.

## Project Description

## Repository Content

* **Adult_Income.ipynb**: The main notebook containing the entire code (EDA, Feature Engineering, Modeling, Stacking).
* **adult.csv**: The raw dataset used for the analysis.
* **profile.html**: Detailed exploratory analysis report (generated via YData Profiling).
* **requirements.txt**: List of necessary dependencies.
* **source/**: Directory containing the LaTeX source code for the project report (main.tex, chapters, bibliography, etc.).

## Technologies and Methodology

The project follows a complete Data Science pipeline using advanced libraries:

1. Exploratory Data Analysis (EDA)
Usage of Pandas and YData Profiling (profile.html) as well as interactive visualizations with Plotly.

2. Modeling (Machine Learning)
We tested and compared several algorithms, including advanced boosting methods:
* Base Models: Logistic Regression, Naive Bayes.
* Ensemble Methods: Random Forest, XGBoost, LightGBM, CatBoost.
* Advanced Technique: Stacking (Meta-model).

3. Optimization
Usage of Optuna to search for the best hyperparameters.

## Conclusion & Key Takeaways

We determined that the **Matthews Correlation Coefficient (MCC)** was the most reliable metric for our evaluation. Unlike Accuracy or F1-Score, MCC provided a more robust measure of the models' quality, particularly given the imbalanced nature of the dataset.

## Authors

* Bonifas Olivier
* Filloux Louis
* Gendronneau Maël

This project was realized within an academic framework.
