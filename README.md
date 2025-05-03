# Kaggle-Titanic---Machine-Learning---Random-Forest-78.708-
Predict Titanic survival using targeted feature engineering (Cabin presence, FamilySize, IsAlone, Title, Age bins) and compare popular models (RF, SVM, KNN, XGBoost, LightGBM). Feature engineering lifted accuracy from \~72% to \~78%. Full code, notebooks, and instructions are available in the GitHub repo.

# Titanic Survival Prediction

This repository contains a full end-to-end analysis and modeling workflow for the classic Titanic Kaggle challenge. It includes:

- **Detailed EDA**  
  A Jupyter notebook that walks through exploratory data analysis:  
  - Summary statistics  
  - Missing-value patterns  
  - Feature distributions and pairwise relationships  
  - Correlation heatmaps

- **Feature Engineering**  
  Creation of high-signal features from raw inputs, including:  
  - `Has_Cabin` (binary cabin indicator)  
  - `FareBin` (quantile-based fare categories)  
  - Group-median imputation for `Age`, then 10-year age bins  
  - `FamilySize` and `IsAlone` derived from SibSp/Parch  
  - `Title` extracted and consolidated from passenger names  

- **Model Comparison**  
  Training and evaluation of multiple classifiers on the engineered feature set:  
  - Random Forest  
  - Support Vector Machine  
  - K-Nearest Neighbors (k=3,5,7)  
  - XGBoost  
  - LightGBM  

  Results are compared side-by-side with a clean bar chart, and each model’s strengths and weaknesses are discussed in detailed Markdown cells.

- **Analysis & Interpretation**  
  Inline Markdown commentary explains:  
  - Why each feature matters  
  - How missing data were handled  
  - The rationale for model selection  
  - Key takeaways and next-step recommendations

## Repository Structure
├── data/
│ ├── train.csv # Official Kaggle training set
│ └── test.csv # Official Kaggle test set
├── notebooks/
│ └── titanic_analysis.ipynb
│ • EDA, feature engineering, model training
│ • Detailed Markdown analysis
├── README.md # Project overview and instructions

## Contributing
Feel free to open issues, fork the repository, or submit pull requests with enhancements—whether it’s new feature ideas, alternative modeling approaches, or visualization improvements.
