📊 Key_Influencers – Logistic Regression-Based Driver Analysis for Attrition
📌 Overview
This project replicates the Key Influencers visualization from Power BI using a custom-built logistic regression model in Python. Power BI’s Key Influencers visual is disabled when using Live Connection or DirectQuery, limiting its use in real-time reporting scenarios.

This tool bridges that gap by using interpretable machine learning to analyze key drivers of employee attrition, making it possible to surface insights in live-mode dashboards or export visuals.

🎯 Objective
Identify the top features that influence employee attrition
Using a logistic regression model, we assess which factors (e.g., job satisfaction, overtime, role, department) significantly increase or decrease the probability of an employee leaving the organization.

📂 Use Case
📉 Predict and explain employee attrition (yes/no) from HR datasets

📊 Replicate Power BI’s Key Influencers visual manually

⚡ Use this in live dashboards where Power BI’s built-in visual is disabled

🔎 Provide HR teams with interpretable insights on what drives employee churn

🧠 How It Works
Input Dataset

Any HR attrition dataset (e.g., IBM’s HR dataset or market samples)

Includes categorical and numerical features

Data Preprocessing

One-hot encoding of categorical variables

Feature scaling (StandardScaler)

Missing value handling

Modeling

Fit a Logistic Regression model with the target: Attrition (Yes/No)

Extract feature coefficients to understand influence direction

Compute odds ratios for interpretability

Visualization

Sorted bar chart of top positive and negative influencers

Export visuals for use in Power BI dashboards or presentations

⚙️ Setup Instructions
bash
Copy
Edit
# Clone the repository
git clone https://github.com/your-username/Key_Influencers_Attrition.git
cd Key_Influencers_Attrition

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebooks/key_influencers_attrition.ipynb
✅ Features
🔍 Analyze binary classification problems like attrition

💡 Understand which features drive outcomes using coefficient-based logic

📤 Export plots for Power BI integration

🧩 Easily customizable to other domains (e.g., churn, conversion, default)

🔄 Future Enhancements
Integrate SHAP values for deeper interpretability

Extend to tree-based models (e.g., XGBoost + feature importance)

Create a Power BI Python visual that auto-loads model output

📬 Contact
Built by Sujoy Sen
For any questions or suggestions, feel free to reach out or raise an issue in the repo.
