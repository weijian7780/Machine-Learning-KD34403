# Machine Learning for Data Science GP

[![Open in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14RSgul4hqc0jZ2QW7bbHLPFE2temYjf8)

## Project Overview

This project is developed for **KD34403 Machine Learning for Data Science**.  
The purpose of this project is to design, implement, test, and document a complete machine learning pipeline using Google Colab.

The notebook demonstrates a machine learning workflow using the **Online Shoppers Purchasing Intention Dataset**. The project focuses on data preprocessing, exploratory data analysis, model training, hyperparameter tuning, and final evaluation. Two machine learning models — Logistic Regression and Random Forest — are trained and compared to determine how well they can predict whether an online shopping session will generate revenue.

## Problem Statement

E-commerce platforms generate large amounts of session data from online visitors. Not all visits result in a purchase, and understanding which sessions are likely to generate revenue is valuable for business analysis.

The main problem is to determine whether machine learning models can correctly predict whether a user session results in revenue (`Revenue = True`) based on behavioural and session-level features.

Since the target class is imbalanced (only ~16% of sessions result in revenue), the project pays special attention to **recall** — capturing as many actual buyers as possible — to support downstream buying-habit analysis.

## Objectives

The objectives of this project are:

1. To load, clean, and preprocess the Online Shoppers Purchasing Intention Dataset for machine learning.
2. To perform exploratory data analysis and visualize important patterns and relationships in the dataset.
3. To train, tune, and compare Logistic Regression and Random Forest models using a proper train/validation/test workflow.
4. To evaluate the final models on an unseen test set and select the best-performing model based on recall and F1-score.

## Dataset Description

The project uses the **Online Shoppers Purchasing Intention Dataset** from the UCI Machine Learning Repository.

- **Source:** [UCI ML Repository](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset)
- **Size:** 12,330 sessions × 18 features
- **Target Variable:** `Revenue` (binary: `True` / `False`)
- **Class Distribution:** ~84% No Revenue, ~16% Revenue

### Features

| Group | Features |
|---|---|
| Page Types & Time Spent | `Administrative`, `Administrative_Duration`, `Informational`, `Informational_Duration`, `ProductRelated`, `ProductRelated_Duration` |
| Google Analytics Metrics | `BounceRates`, `ExitRates`, `PageValues` |
| Session Details | `SpecialDay`, `Month`, `OperatingSystems`, `Browser`, `Region`, `TrafficType`, `VisitorType`, `Weekend` |
| Target Variable | `Revenue` |

## Machine Learning Pipeline

The project follows a complete machine learning pipeline:

```text
Raw Dataset
     ↓
Data Loading
     ↓
Data Cleaning and Preprocessing
     ↓
Exploratory Data Analysis
     ↓
Train / Validation / Test Split (60 / 20 / 20)
     ↓
Baseline Model Training
     ↓
Hyperparameter Tuning (GridSearchCV)
     ↓
Model Evaluation on Test Set
     ↓
Final Result and Conclusion
```

## Project Files

```text
.
├── README.md
├── Machine Learning for Data Science GP.ipynb
├── data/
│   └── online_shoppers_intention.csv
├── images/
│   └── visualizations.png          # Optional, for charts or result screenshots
└── requirements.txt                # Optional, for Python package list
```

## How to Run the Project

### Run in Google Colab (Recommended)

1. Open the Google Colab notebook using the badge at the top of this README.
2. Upload `online_shoppers_intention.csv` to `/content/` in the Colab file browser.
3. Click **Runtime → Run all**.
4. Check the output of each section.
5. Review the final model comparison and evaluation results in Milestone 5.

## Technologies Used

| Tool / Library | Purpose |
|---|---|
| Google Colab | Cloud-based notebook environment |
| Python 3 | Programming language |
| Pandas | Data loading and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Seaborn | Statistical visualisation |
| Scikit-learn | ML pipelines, preprocessing, models, and evaluation |

## Milestone Progress

This project follows the KD34403 machine learning workflow milestones.

| Milestone | Description | Status |
|---|---|---|
| Milestone 1 | Data Pipeline: dataset loading, EDA, visualisations, preprocessing | ✅ Completed |
| Milestone 2 | Architecture Logic: model choice, pipeline design, and explanation | ✅ Completed |
| Milestone 3 | Training Loop: train/val/test split, baseline training, initial metrics | ✅ Completed |
| Milestone 4 | Model Optimisation: GridSearchCV, depth regularisation, threshold analysis | ✅ Completed |
| Milestone 5 | Final Evaluation: test set metrics, confusion matrices, model decision | ✅ Completed |

## Supporting Materials

| Item | Link |
|---|---|
| Milestone 1 YouTube Video | https://www.youtube.com/watch?v=U8iT_4e9q8g |
| Milestone 2 YouTube Video | https://www.youtube.com/watch?v=-6_WGQIlX4g |
| Milestone 3 YouTube Video | https://www.youtube.com/watch?v=6hjbIY2piiA |
| Milestone 4 YouTube Video | https://www.youtube.com/watch?v=jIoXQ9dMXek |
| Milestone 5 YouTube Video | https://www.youtube.com/watch?v=u48QuUqXTCI |
| GitHub Repository | https://github.com/weijian7780/Machine-Learning-KD34403 |
| Google Colab Notebook | https://colab.research.google.com/drive/14RSgul4hqc0jZ2QW7bbHLPFE2temYjf8 |

## Contributors

| Name | Role |
|---|---|
| LIM JIA LEONG | Milestone 1 |
| YUGEINDRAN A/L TANDAUTABANI | Milestone 2 |
| CHEN WEI JIAN | Milestone 3 |
| CHIA ZHENG XUN | Milestone 4 |
| LEE YI YUEN | Milestone 5 |
| All Students | Poster and GitHub |

## License

This project is created for academic purposes under KD34403 Machine Learning for Data Science.
