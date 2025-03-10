# March Madness Machine Learning Predictor  
**Exploring NCAA Tournament Predictions with Machine Learning**

## Overview  
This project builds a machine learning model to predict NCAA Tournament winners using historical team statistics and matchup data. It consists of:

- **Data Preprocessing**: Cleans and prepares team matchup data for analysis
- **Exploratory Data Analysis (EDA)**: Investigates key patterns in team performance metrics
- **Model Development**: Trains and compares multiple machine learning algorithms
- **Model Evaluation**: Evaluates performance using various classification metrics

Key insights from the EDA:
- Dataset contains 358 historical matchups with 26 features
- Wins are slightly more common than losses (58% vs 42% distribution)
- Features include offensive/defensive efficiency, team ratings, experience levels, and BPI rankings

## Project Structure  
**march_code_pudding.ipynb** - Main notebook containing:
1. Data Import & Preprocessing
   - Handles missing values
   - Removes duplicates
   - Renames target column
2. Exploratory Data Analysis
   - Class distribution visualization
   - Feature distribution analysis
   - Statistical summary of key metrics
3. Model Development
   - Trains CatBoost
   - Includes hyperparameter tuning
4. Model Evaluation
   - Compares accuracy, precision, recall, F1-score, and ROC-AUC
   - Feature importance analysis

## Datasets  
**team_matchups.csv** - Contains:
- 26 features including:
  - Team rankings (BPI, offensive/defensive efficiency)
  - Game statistics (points scored, tempo)
  - Experience metrics
  - Historical matchup outcomes
- 358 cleaned records of historical team matchups

## Key Features  
- **Comprehensive Data Analysis**: Detailed exploration of team performance metrics
- **Multiple Model Comparison**: Evaluates 1 machine learning algorithm
- **Model Interpretation**: Accuracy score analysis
- **Class Balancing**: Handles imbalanced outcomes using resampling techniques

## Tech Stack  
- **Python**  
- **Jupyter Notebook**  
- **Data Processing**: Pandas, NumPy  
- **Visualization**: Matplotlib, Seaborn  
- **Machine Learning**: 
  - Scikit-learn
  - CatBoost
- **Statistical Analysis**: SciPy

## Installation  
1. Clone repository
2. Install dependencies:
```bash
pip install catboost pandas matplotlib seaborn numpy scikit-learn
