🩺 Diabetes Risk Prediction — Machine Learning & Deep Learning with XAI
This project contains the modelling work from my MSc dissertation, reframed as a clean, portfolio-quality machine learning case study.
The goal is simple: predict early diabetes risk using clinical features, compare ML and deep learning models, and explain the predictions clearly.
This project covers:
Classical ML (Logistic Regression, Random Forest, XGBoost)
Deep learning models (ANN, CNN, LSTM)
Full data prep pipeline
Model evaluation and comparison
Explainability using SHAP and LIME
The focus is accuracy, interpretability, and real-world usa

🔍 Project objective
Early detection of diabetes significantly reduces long-term complications.
This project explores whether machine learning models can identify high-risk patients using a structured clinical dataset.
Key goals:
Build multiple ML & DL models
Compare performance across metrics
Analyse feature importance
Explain predictions using XAI
Identify the most clinically relevant predictors

📂 Project structure
Diabetes-Prediction/
│
├── data/                     # dataset or schema (if restricted)
├── notebooks/
│     ├── 01_eda.ipynb        # data exploration
│     ├── 02_preprocessing.ipynb
│     ├── 03_ml_models.ipynb  # Logistic Regression, RF, XGBoost
│     ├── 04_dl_models.ipynb  # ANN, CNN, LSTM
│     ├── 05_xai_shap.ipynb   # SHAP explainability
│     └── 06_lime_explain.ipynb
│
├── models/                   # saved models
├── reports/
│     └── dissertation_summary.pdf

🧪 Data

The dataset contains anonymised patient diagnostic and lifestyle features relevant to diabetes risk prediction, including:
Age
BMI
Blood pressure
Glucose level
Insulin
Skin thickness
Pregnancies (for female patients)
Diabetes pedigree
Outcome (0/1)
If the original dataset is private/restricted, the repository includes either a public alternative (e.g., UCI Pima Indians Diabetes dataset) or a schema-only description.

⚙️ Models implemented
Classical ML
Logistic Regression
Random Forest
XGBoost
Gradient Boosting
SVM (optional)
Deep Learning
Feedforward ANN
CNN (for feature patterns)
LSTM (for temporal/sequence-style modelling — adapted version)
Each model is trained, tuned, and evaluated using cross-validation.

📊 Evaluation
Metrics included:
Accuracy
Precision
Recall
F1-score
ROC-AUC
Confusion matrix
Key findings:
LSTM model achieved the best performance, with an F1-score around ~0.94 (based on the original dissertation dataset).
Tree-based models (Random Forest / XGBoost) performed competitively and offer easier interpretability.
Logistic Regression serves as a strong baseline.

🧠 Explainability (XAI)
Explainability is essential for clinical decision-making.
The project includes:
✔️ SHAP (global + local)
Identifies the top contributors to risk
Shows whether each feature increases or decreases predicted risk
Provides per-patient explanations
✔️ LIME
Localised explanations for individual predictions
Good for case-by-case clinical review
Common findings:
Glucose level
BMI
Age
Blood pressure
were consistent top drivers of diabetes risk.

▶️ How to run
Install dependencies:
pip install -r requirements.txt
Run notebooks in order:
01_eda.ipynb → explore data
02_preprocessing.ipynb → build clean dataset
03_ml_models.ipynb → ML training
04_dl_models.ipynb → deep learning training
05_xai_shap.ipynb → SHAP analysis
06_lime_explain.ipynb → LIME analysis

🚀 Future improvements
Hyperparameter optimisation with Optuna
Probability calibration for clinical deployment
Fairness analysis across demographic subgroups
Conversion into a Streamlit dashboard
Integrating real-world EHR features if available

📘 Summary
This project demonstrates an end-to-end ML pipeline for diabetes prediction, including:
✔️ Solid classical + deep learning models
✔️ Full data preparation
✔️ Strong evaluation and interpretation
✔️ Clinically meaningful insights
✔️ Proper explainability with SHAP and LIME
It reflects both academic depth and practical implementation.
│
├── requirements.txt
└── README.md
