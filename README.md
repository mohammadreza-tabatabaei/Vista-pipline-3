# Phishing URL Detection

This project focuses on detecting phishing URLs using machine learning models trained on a rich set of engineered features extracted from the structure and metadata of URLs.

## 📁 Dataset
The dataset contains 112 features that represent:
- Character frequencies and structural patterns in different URL components (domain, path, file, parameters)
- Network-based features (TTL, SSL certificate presence, DNS info)
- Behavioral traits (number of redirects, Google indexing, use of shortened URLs)
- Label: `phishing` (1 = phishing, 0 = legitimate)

## 🧠 Models Used
- **Random Forest Classifier**
- **XGBoost Classifier**

Both models were trained and evaluated using scikit-learn and XGBoost.

## 📊 Feature Analysis
- **Correlation heatmap** was used to identify top features strongly associated with phishing.
- **SHAP (SHapley Additive exPlanations)** summary and waterfall plots were generated to explain model predictions at global and local levels.
- **LIME (Local Interpretable Model-agnostic Explanations)** was also used to visualize individual prediction decisions.

## 🧪 Evaluation
- Models were evaluated using accuracy and classification reports.
- Feature importance visualizations helped interpret how each model makes decisions.

## 📂 Files
- `URL_DETECT.ipynb` – Jupyter notebook with full training and analysis pipeline.
- `url_detect.py` – Script version for streamlined execution.
- `phishing-dataset-variation.csv` – The dataset used.

## ✅ Requirements
- Python 3.x
- pandas, numpy, scikit-learn, xgboost, shap, lime, seaborn, matplotlib

## 🚀 How to Run
1. Clone the repository
2. Install dependencies
3. Run the Jupyter notebook or execute `url_detect.py`

## 📌 Goal
To develop a robust, interpretable machine learning pipeline for identifying malicious URLs based on structural and contextual cues.
