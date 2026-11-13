# 🩸 Anemia Classification & Diagnostics System

[![Python Version](https://img.shields.io/badge/Python-3.10%2B-blue.svg?style=for-the-badge&logo=python)](https://www.python.org)
[![ML Accuracy](https://img.shields.io/badge/Model_Accuracy-100%25-success.svg?style=for-the-badge&logo=scikit-learn)](https://scikit-learn.org)
[![Gradio App](https://img.shields.io/badge/UI-Gradio_Demo-orange.svg?style=for-the-badge&logo=gradio)](https://gradio.app)

An end-to-end Machine Learning and Diagnostics dashboard designed to classify individuals into **Anemic**, **Non-Anemic**, or **Compensated Microcytosis** classes based on Complete Blood Count (CBC) parameters.

---

## 🗺️ Project Architecture & Workflow

[ Raw CSV Data ] ──> [ Data Cleaning & PCT Recalculation ] ──> [ Exploratory Data Analysis ] │ [ Gradio Web UI ] <── [ Saved Artifacts (.pkl) ] <── [ Decision Tree (100% Acc) ] ◄────┘


---

## 🔬 Key Insights & Highlights

* **Feature Optimization**: Out of 23 original features, the system is optimized to use only the top 4 highly predictive features (`HGB`, `MCH`, `RDW_CV`, and `Gender`) without any loss in diagnostic accuracy.
* **Perfect Class Separation**: The Decision Tree model achieves **100% accuracy** (cross-validated), demonstrating distinct boundaries between physiological patient classes.
* **Dynamic UI**: Built with a production-ready Web Interface powered by Gradio, allowing real-time clinical entry predictions.

---

## 🚀 Quick Start & Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/anemia-classification-system.git
cd anemia-classification-system
2. Install Dependencies
pip install -r requirements.txt
3. Launch the Web Interface
python app.py
📊 Feature Profiles & Diagnostic Impact
Based on Exploratory Data Analysis, red-cell profiles behave distinctly across patient classes:

Anemic: Marked by a significant drop in Hemoglobin (HGB median ~10.9 g/dL) and low MCV / MCH.
Compensated Microcytosis: Exhibits normal-to-borderline Hemoglobin (median ~13.9 g/dL) but accompanied by microcytic red cell features (lower MCV/MCH).
Non-Anemic: Optimal hematological parameters (HGB median ~14.4 g/dL, normal MCV).
🛠️ Tech Stack & Libraries Used
Core Analysis: Pandas, NumPy
Visualization: Matplotlib, Seaborn, Plotly Express
Machine Learning: Scikit-Learn (StandardScaler, DecisionTreeClassifier, LogisticRegression)
Deployment: Gradio, Pickle
Developed as a diagnostic and analytical toolkit for hematological research. ```
