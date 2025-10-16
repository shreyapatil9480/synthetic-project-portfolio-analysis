# Project Portfolio Analysis

This repository contains a synthetic dataset and analysis notebook for exploring project portfolio performance. The goal is to showcase skills relevant to **Business Analysts**, **Program Managers**, and **Data Analysts** by performing data exploration, visualization, and predictive modeling on project-related data.

## Repository Structure

- **synthetic_project_data.csv** – Synthetic dataset with 500 projects. Each row represents a project with features such as department, manager experience, team size, complexity, planned vs. actual durations and budgets, and satisfaction score.
- **analysis.ipynb** – Jupyter notebook that loads the dataset, performs exploratory data analysis (EDA), visualizes relationships between variables, and builds predictive models (Linear Regression and Random Forest) to estimate project satisfaction scores.
- **requirements.txt** – List of Python dependencies needed to run the notebook.

## Dataset Overview

The synthetic dataset simulates various aspects of project management:

| Column | Description |
|-------|-------------|
| project_id | Unique identifier for each project |
| department | Department responsible for the project (e.g., IT, HR, Finance, etc.) |
| manager_experience_years | Years of experience of the project manager |
| team_size | Number of people in the project team |
| complexity_score | A score (1–10) representing project complexity |
| planned_duration_months | Planned duration of the project in months |
| actual_duration_months | Actual duration of the project in months |
| planned_budget_k | Planned budget (in thousands) |
| actual_budget_k | Actual budget (in thousands) |
| satisfaction_score | Satisfaction rating (1–10) influenced by budget and schedule performance |

## Getting Started

1. **Clone this repository**

   ```bash
   git clone https://github.com/shreyapatil9480/synthetic-project-portfolio-analysis.git
   cd synthetic-project-portfolio-analysis
   ```

2. **Set up a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the notebook**

   You can run the analysis notebook using Jupyter:

   ```bash
   jupyter notebook analysis.ipynb
   ```

   Alternatively, execute the notebook from the command line:

   ```bash
   jupyter nbconvert --to notebook --execute analysis.ipynb --inplace
   ```

## Analysis Highlights

- **Exploratory Data Analysis (EDA)**: Examine the distribution of variables, correlations, and department-wise satisfaction scores.
- **Visualization**: Generate a pairplot for numeric features, a correlation heatmap, and box plots to identify patterns and outliers.
- **Predictive Modeling**: Build and compare Linear Regression and Random Forest models to predict the satisfaction score based on project attributes.
- **Evaluation**: Assess model performance using metrics like MAE, RMSE, and R2 score.

## Future Work

This project can be extended by:

- Adding more realistic constraints or features to the synthetic dataset.
- Exploring classification problems (e.g., predicting on-time vs. delayed projects).
- Implementing hyperparameter tuning for the Random Forest model or experimenting with advanced models like Gradient Boosting or XGBoost.

Feel free to explore the dataset, modify the notebook, and contribute improvements!

## How to Interpret Results

The predictive models in this project estimate a satisfaction score based on project attributes. A higher satisfaction score suggests better alignment with schedule and budget expectations. When interpreting the results:

- **Linear Regression**: Provides an interpretable baseline, showing the strength and direction of relationships between features and satisfaction score. Use the coefficients to understand which factors most influence satisfaction.
- **Random Forest**: Captures non-linear relationships and interactions. The feature importance plot highlights which attributes (e.g., budget variance, team size) most affect the score.

By comparing model performance metrics (MAE, RMSE, R²), you can assess which model generalizes best to unseen data.

