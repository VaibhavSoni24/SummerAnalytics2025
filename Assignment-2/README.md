# 🌱 NDVI Land Cover Classification - Summer Analytics 2025

This repository contains my submission for the **First Course Hackathon** hosted by **Consulting & Analytics Club** and **GeeksforGeeks** as part of **Summer Analytics 2025**.

## 📌 Problem Statement
Use NDVI (Normalized Difference Vegetation Index) time-series data to classify land cover types into categories such as:
- Water
- Impervious
- Farm
- Forest
- Grass
- Orchard

Model used: **Multiclass Logistic Regression** (only model allowed)

## 🧠 Approach

- **Missing Value Handling**: Mean imputation of NDVI values
- **Feature Engineering**: Extracted `mean`, `std`, `min`, `max`, and `range` from 27 NDVI time-series columns
- **Scaling**: Standardized features using `StandardScaler`
- **Model**: Trained a Logistic Regression model (`saga` solver, multinomial class)
- **Validation Accuracy**: ~92.06%
- **Prediction**: Used model to classify the test set

## 📂 Repository Contents

| File Name              | Description                                      |
|------------------------|--------------------------------------------------|
| `hacktrain.csv`        | Training dataset provided by the competition     |
| `hacktest.csv`         | Test dataset provided by the competition         |
| `program.py`           | Python code to preprocess, train, and predict    |
| `data.csv`             | Final submission file (ID + predicted class)     |

## 📈 Evaluation
Final submission evaluated based on **classification accuracy**.

---

**Author**: Vaibhav Soni  
**Event**: Summer Analytics 2025 – CAC, IIT Guwahati  
