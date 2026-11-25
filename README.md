# Bootcamp Project: Customer Lifetime Churn Prediction

## 📌 Project Overview
This project leverages statistical modeling and machine learning to predict customer churn and optimize Lifetime Value (LTV) for an e-commerce subscription platform. By analyzing historical transaction patterns, the models identify at-risk users and provide actionable insights for targeted retention strategies and enhanced customer experience.

## 📊 Dataset Description
The analysis utilizes datasets located in the `data/` directory:
* **`customers.csv`**: Contains user metadata including `customer_id`, `signup_date`, and `true_lifetime_days`.
* **`transactions.csv`**: Raw logs of every purchase made by customers, including `customer_id`, `transaction_date`, and `amount`.
* **`transaction_summary.csv`**: Aggregated features generated via the BG/NBD model for use in downstream analysis.

## 🛠️ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Bao-Tien2k6/customer-lifetime-churn.git](https://github.com/Bao-Tien2k6/customer-lifetime-churn.git)
    cd customer-lifetime-churn
    ```
2.  **Set up virtual environment:**
    ```bash
    python -m venv venv
    # Activate on Windows:
    .\venv\Scripts\activate
    # Activate on macOS/Linux:
    source venv/bin/activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## 🚀 Usage
Notebooks in the `model/` directory can be executed independently; however, the following workflow is recommended:
1.  Run **`bg_nbd.ipynb`** first to generate the `transaction_summary.csv` file.
2.  Use the generated summary for **`survival_analysis.ipynb`** and **`clv_modelling.ipynb`**.

## 🏗️ Project Structure
```text
├── .vscode/               # VS Code workspace settings
├── data/                  # Source datasets and generated summaries
│   ├── customers.csv
│   ├── transaction_summary.csv
│   └── transactions.csv
├── data_analysis/         # Exploratory Data Analysis (EDA)
├── model/                 # Statistical and ML notebooks
│   ├── bg_nbd.ipynb       # Probability models for transaction frequency
│   ├── churn_prediction.ipynb
│   ├── clv_foundations.ipynb
│   ├── survival_analysis.ipynb
│   └── clv_modelling.ipynb
├── outcome/               # Model outputs and performance reports
└── README.md
