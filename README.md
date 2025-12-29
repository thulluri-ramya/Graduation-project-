📌 Project Overview

Cervical cancer remains one of the most preventable yet life-threatening cancers affecting women worldwide, particularly in regions with limited access to regular screening and diagnostic facilities. Early detection plays a crucial role in reducing mortality; however, traditional screening methods may not always be accessible or affordable.

This project applies machine learning techniques to predict cervical cancer biopsy outcomes using behavioural, demographic, and clinical risk factors. The objective is to develop an interpretable and recall-focused predictive model that can support early risk identification and clinical decision-making, especially in low-resource settings.

The project forms part of the MSc Data Science final project at the University of Hertfordshire.

📂 Dataset

Source: UCI Machine Learning Repository

Dataset Name: Cervical Cancer (Risk Factors)

Records: 858 patients

Features: 36 behavioural, demographic, and medical attributes

Target Variable: Biopsy (0 = Negative, 1 = Positive)

Feature Categories:

Demographic information (e.g., age)

Sexual and reproductive history

Smoking behaviour

Hormonal contraceptive and IUD usage

Sexually transmitted disease (STD) indicators

Preliminary screening test results

⚙️ Methodology

The project follows a structured machine learning pipeline:

Data Exploration

Missing value analysis

Feature distribution visualisation

Data Preprocessing

Median and mode imputation for missing values

Feature scaling using StandardScaler

Binary encoding for categorical variables

Train–Test Split

70% training, 30% testing

Stratified to preserve class distribution

Model Development

Logistic Regression

Decision Tree

Random Forest

Support Vector Machine (SVM)

XGBoost

Artificial Neural Network (ANN)

Model Evaluation

Accuracy

Precision

Recall (primary metric)

F1-score

Confusion matrices

📊 Key Results

Tuned Logistic Regression achieved the highest recall (~87%)

Ensemble models (Random Forest, XGBoost) showed high accuracy but lower sensitivity

ANN performance was limited due to dataset size

Logistic Regression was selected as the most clinically suitable model due to:

High recall

Interpretability

Computational efficiency

🧠 Feature Importance

Feature importance analysis identified key predictors aligned with known cervical cancer risk factors, including:

STD history

Smoking behaviour

Age at first sexual intercourse

Number of sexual partners

Contraceptive usage

These findings support the clinical relevance of the dataset and model outputs.

🧪 Technologies & Libraries Used

Programming Language: Python

Libraries:

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

XGBoost

TensorFlow / Keras

📁 Repository Structure
├── data/
│   └── cervical_cancer_DS.xlsx
├── notebooks/
│   └── cervical_cancer_ml.ipynb
├── figures/
│   └── confusion_matrices_and_plots/
├── README.md

🚀 How to Run the Project

Clone the repository:

git clone https://github.com/your-username/Graduation-project-


Install required dependencies:

pip install -r requirements.txt


Run the Jupyter Notebook:

jupyter notebook

🔐 Ethical Considerations

This project uses anonymised, publicly available data. The models are intended as decision-support tools, not replacements for clinical diagnosis. Emphasis is placed on minimising false negatives to support patient safety.

📌 Future Work

Address class imbalance using techniques such as SMOTE

Validate models on larger and more diverse datasets

Integrate explainable AI (XAI) methods

Combine behavioural data with imaging or genomic features

👩‍🎓 Author

Ramya Thulluri
MSc Data Science
University of Hertfordshire

🔗 GitHub Repository: Linked in project report
