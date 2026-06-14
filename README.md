# 📊 Key Influencers – Logistic Regression-Based Driver Analysis for Attrition

A machine learning solution that replicates Power BI's **Key Influencers** visualization using **Logistic Regression**, enabling interpretable driver analysis even when Power BI's native visual is unavailable in **Live Connection** or **DirectQuery** mode.

---

## 🎯 Project Goal

Identify and explain the factors that most strongly influence employee attrition.

By leveraging Logistic Regression and coefficient-based interpretation, the project highlights which employee attributes increase or decrease the likelihood of attrition, providing HR teams with actionable insights.

---

## 🚀 Why This Project?

Power BI's built-in **Key Influencers** visual is disabled in several real-world reporting scenarios, particularly when using:

* Live Connection
* DirectQuery
* Certain enterprise reporting environments

This project provides an alternative approach by generating interpretable machine learning insights that can be integrated directly into dashboards and reports.

---

## ✨ Key Features

* 🔍 Analyze employee attrition drivers using Logistic Regression
* 📈 Replicate Power BI's Key Influencers visual through custom modeling
* 💡 Interpret feature impact using coefficients and odds ratios
* 📤 Export visualizations for Power BI integration
* ⚡ Compatible with live reporting workflows
* 🧩 Easily adaptable to churn, conversion, risk, and default prediction problems

---

## 📂 Business Use Case

This project can be used to:

* Understand employee turnover patterns
* Identify high-risk attrition factors
* Support HR decision-making with interpretable insights
* Generate explanatory visuals for executive reporting
* Enable influencer analysis in environments where Power BI visuals are restricted

---

## 🧠 Methodology

### 1. Data Input

The model accepts HR datasets containing:

* Employee demographics
* Job-related attributes
* Satisfaction metrics
* Attrition labels

Example datasets:

* IBM HR Analytics Dataset
* Market HR Attrition Datasets

---

### 2. Data Preprocessing

The pipeline performs:

* One-hot encoding of categorical variables
* Feature scaling using StandardScaler
* Missing value handling
* Data preparation for modeling

---

### 3. Logistic Regression Modeling

Target Variable:

```text
Attrition (Yes / No)
```

The model:

* Learns relationships between employee attributes and attrition
* Calculates feature coefficients
* Generates odds ratios for business-friendly interpretation

---

### 4. Influencer Analysis

Feature importance is derived from Logistic Regression coefficients.

The output identifies:

* Factors increasing attrition probability
* Factors reducing attrition probability
* Relative impact strength of each feature

---

### 5. Visualization

Generated outputs include:

* Top positive influencers
* Top negative influencers
* Sorted coefficient visualizations
* Exportable charts for Power BI dashboards

---

## 🏗️ Project Workflow

```text
HR Dataset
      │
      ▼
Data Preprocessing
      │
      ▼
Logistic Regression Model
      │
      ▼
Coefficient Analysis
      │
      ▼
Odds Ratio Calculation
      │
      ▼
Influencer Visualization
      │
      ▼
Power BI Integration
```

---

## ⚙️ Installation & Setup

### Clone Repository

```bash
git clone https://github.com/your-username/Key_Influencers_Attrition.git
cd Key_Influencers_Attrition
```

### Create Virtual Environment (Optional)

```bash
python -m venv venv
```

Windows:

```bash
venv\Scripts\activate
```

Linux / macOS:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Notebook

```bash
jupyter notebook notebooks/key_influencers_attrition.ipynb
```

---

## 📈 Sample Outputs

* Employee attrition driver rankings
* Logistic Regression coefficient analysis
* Odds ratio interpretation charts
* Power BI-ready visual exports

---

## 🔄 Future Enhancements

* SHAP-based explainability
* Tree-based models (Random Forest / XGBoost)
* Automated Power BI Python Visual integration
* Interactive dashboard generation
* Model comparison framework

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

---

## 👨‍💻 Author

**Sujoy Sen**

Computer Science Engineering Student | Machine Learning & Data Analytics Enthusiast

Feel free to open an issue or contribute improvements to the project.

---

## 📄 License

This project is intended for educational and analytical purposes.
