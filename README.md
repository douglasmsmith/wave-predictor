## Wave Height Prediction Project

This project aims to predict perceived wave heights using data from an offshore buoy. It serves to demonstrate
my skills in data preprocessing, exploratory data analysis, feature engineering and predictive modeling.

## Summary of Results

The preprocessing notebook (00) was adapted from the original preprocessing notebook provided. Data exploration (01)
investigates the preprocessed data. I adapted these two notebooks throughout the project, as I gained more insight into
potentially useful features.

After a preliminary analysis of feature importance using a random forest (02), I decided to frame the problem as a regression task, with a view to rounding predictions to match the discreteness of the human observation targets. I started with a simple linear regression model as a baseline (03) and then conducted a comparison of this model against three others models (04).

Given that XGBoostRegressor showed the most promise at the model comparison stage, I focuse on improving this model through hyperparamter tuning, during which I employed a grid searchs strategy (05). In this final notebook, I summarise my findings and considerations for future work on this dataset.

## Setup

1. Clone this repository.
2. Create a conda environment: `conda create --name surf_env`.
3. Activate the environment: `conda activate surf_env`.
4. Install dependencies in `requirements.txt`.
5. Run Jupyter notebooks in the `notebooks/` directory.

## Project Structure

- `data/`: Contains raw and processed data files.
- `notebooks/`: Jupyter notebooks for data preprocessing, analysis and modeling.
- `requirements.txt`: List of Python package dependencies.
