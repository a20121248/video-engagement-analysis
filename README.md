# Video Engagement Analysis
Statistical analysis of video like/dislike patterns using Python and machine learning.

## Overview
This project analyzes 344K user interactions to understand what drives video engagement across different platforms and content types.

## Key Findings
- **Platform Effect**: iPhone users 30% more likely to like videos than Roku users
- **Personalization Works**: Both favorites → 84% like rate vs 49% baseline  
- **Timing Matters**: Peak engagement during 5-8 AM window
- **Content Strategy**: Short videos from top authors perform best

## Files
```
notebooks/
├── 01_eda.ipynb              # Exploratory data analysis
├── 02_feature_engineering.ipynb  # Feature creation
├── 03_statistical_test.ipynb     # Chi-square significance test
└── 04_logistic_regression.ipynb  # Predictive modeling

data/
└── raw/sample_data.parquet.gzip   # Original dataset
```

## Results
- **Model Performance**: AUC 0.667, Gini 0.333
- **Statistical Significance**: p < 0.001 (highly significant)
- **Top Predictors**: Missing user stats (+58%), Favorite channels (+33%), Premium platforms (+31%)

## Usage
1. Run notebooks in order (01 → 04)
2. Each notebook answers a specific research question
3. Final model identifies key engagement drivers

## Tech Stack
Python • Pandas • Scikit-learn • Statsmodels • Matplotlib • Seaborn