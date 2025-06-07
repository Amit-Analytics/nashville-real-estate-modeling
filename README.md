# Nashville Property Valuation Modeling

This project helps a real estate company identify undervalued and overvalued properties in the Nashville housing market. By building multiple predictive models, the goal is to guide investment decisions using data-driven insights into home pricing trends.

---

## Problem Statement

A real estate firm is preparing to invest significantly in the Nashville area but is concerned that properties may be selling above their actual value. The company provided a dataset of historical sales and asked for an analysis that identifies **undervalued or overvalued homes** based on market data. This project creates a binary classification target to predict such value discrepancies.

---

## Project Objectives

- Clean and preprocess the dataset for analysis
- Engineer a target variable (overpriced/underpriced)
- Train and compare multiple machine learning models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Gradient Boosting
  - Neural Network
  - Ensemble Voting
- Identify which features influence pricing most
- Recommend a model and key investment factors

---

## Task Summary

### Task 1: Data Cleaning
- Removed null values and formatted dates
- Converted text fields to categorical variables
- Engineered binary target variable using `SalePrice` vs. `TotalValue`

### Tasks 2–6: Model Training
Built and tuned the following models to classify homes as overpriced or underpriced:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting Classifier
- Neural Network (MLPClassifier)

### Task 7: Model Evaluation

| Model             | Accuracy | Precision | Recall | F1 Score |
|------------------|----------|-----------|--------|----------|
| Logistic Model    | 0.79     | 0.80      | 0.78   | 0.79     |
| Decision Tree     | 0.85     | 0.86      | 0.85   | 0.85     |
| Random Forest     | 0.91     | 0.91      | 0.91   | 0.91     |
| Gradient Boost    | 0.92     | 0.92      | 0.92   | 0.92     |
| Neural Network    | 0.84     | 0.85      | 0.84   | 0.84     |
| Ensemble Voting   | 0.92     | 0.92      | 0.92   | 0.92     |

>  **Recommendation:** The **Gradient Boosting** and **Ensemble Voting** models achieved the highest performance. These models should be used for future predictions, focusing on variables like `YearBuilt`, `TotalValue`, `LandValue`, and `BuildingArea`.

---


## 🛠️ Tools & Libraries

- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Neural Network (MLPClassifier from Scikit-learn)
- Ensemble Modeling (VotingClassifier)
- Jupyter Notebook
- Matplotlib & Seaborn
- Git & GitHub

---

## Repository Structure

```bash
nashville-property-valuation-modeling/
├── Investment_Analysis.ipynb       # Jupyter Notebook with full analysis
├── Investment_Analysis.html        # Exported HTML version
├── Data_Dictionary.docx            # Word document describing feature definitions
├── Housing_housing_data.csv                # (optional: raw dataset)
├── README.md                       # Project documentation
