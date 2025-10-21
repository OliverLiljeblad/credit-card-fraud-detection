# Credit Card Fraud Detection

**Overview**  
This project builds a machine learning model to detect fraudulent credit card transactions.  
It uses techniques for preprocessing, handling imbalanced data, and modeling with XGBoost.  
The goal is to create a reproducible, professional project suitable for learning and demonstrating skills to recruiters.

Skills Demonstrated:
Python (pandas, numpy, scikit-learn, XGBoost)
Data preprocessing and scaling
Handling imbalanced datasets (SMOTE)
Model evaluation (ROC, PR curves, F1-score, classification report)
Feature importance analysis & explainability (SHAP)
End-to-end ML pipeline and deployment simulation
GitHub workflow: notebooks, saved models, results, plots

---

## 📂 Project Structure

credit-card-fraud-detection/
├── 01_EDA.ipynb # Exploratory Data Analysis
├── 02_Preprocessing_and_Modeling.ipynb # Data preprocessing and model training
├── 03_Evaluation_and_Deployment.ipynb # Model evaluation, threshold tuning, and deployment
├── requirements.txt # Project dependencies
├── .gitignore # Ignore dataset, virtualenv, artifacts
├── plots/ # Generated plots (class distribution, ROC curves, etc.)
├── models/ # Saved trained models and scalers
└── results/ # Prediction outputs


---

## ⚙️ Setup Instructions

1. Clone the repo:
```bash
git clone https://github.com/YOUR-USERNAME/credit-card-fraud-detection.git
cd credit-card-fraud-detection

python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

pip install -r requirements.txt

2. 📝 How to Run Jupyter Notebooks

Launch Jupyter Lab or Notebook:
jupyter lab
# or
jupyter notebook

Run notebooks in order:
01_EDA.ipynb → explore dataset
02_Preprocessing_and_Modeling.ipynb → train model
03_Evaluation_and_Deployment.ipynb → evaluate & test model

Python script (optional)
python src/train.py (Not ready)

3. (Not ready)
FastAPI demo (optional)
uvicorn app.api:app --reload --port 8000

Streamlit demo (optional)
streamlit run app/streamlit_app.py

📊 Key Features
Exploratory Data Analysis (EDA)
Handling imbalanced datasets with SMOTE
XGBoost classifier with ROC-AUC evaluation
Threshold tuning for business-aware fraud detection
Model saving/loading with Joblib
Optional FastAPI endpoint and Streamlit demo

⚡ Notes
Dataset is not included in the repo (sensitive data) — place creditcard.csv in project root.
Metrics focus on Precision, Recall, F1-score, and ROC/PR AUC due to imbalanced data.
Recommended workflow: run notebooks top-to-bottom, use virtual environment, follow reproducible practices.

📌 Future Improvements
Hyperparameter tuning with cross-validation
SHAP-based feature explainability
Deploy with Docker or cloud service
Integration into a real-time transaction monitoring system

Work in progress, fine tuning required
