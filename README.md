# Bootcamp Project: Customer Lifetime Churn Prediction

## 📌 Project Overview
Imagine myself as a Data Scientist in an e-commerce company with subscription products. By using statistical analysis, this project aims to predict time to churn and maximize customer lifetime value using historical transaction data. By identifying at-risk customers, businesses can implement targeted retention strategies for customer retention and experience enhancement.

## 📊 Dataset Description
Describe the data files used in this project (as seen in the `data/` folder):
* `customers.csv`: Contains basic user information (customer_id, signup_date, true_lifetime_days).
* `transactions.csv`: Raw logs of every purchase made by customers (customer_id, transaction_date, amount).

## 🛠️ Installation & Setup
Provide clear steps for others to run your code:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Bao-Tien2k6/customer-lifetime-churn.git](https://github.com/Bao-Tien2k6/customer-lifetime-churn.git)
   cd customer-lifetime-churn

2. **Create a virtual environment**
   ```bash
  python -m venv venv
  source venv/bin/activate  # On Windows: venv\Scripts\activate

3. **Install dependencies**
4. **Usage**
   Each model could be run separately. *transaction_summary.csv* is obtained from bg_nbd which will be used in survival analysis and clv_modelling later.

## 🏗️ Project Structure
├── .vscode/               # VS Code workspace settings
├── data/                  # Source datasets
│   ├── customers.csv
│   ├── transaction_summary.csv
│   └── transactions.csv
├── data_analysis/         # Exploratory analysis and data processing
├── model/                 # Machine learning and statistical notebooks
│   ├── bg_nbd.ipynb       # Beta-Geometric/Negative Binomial Distribution model
│   ├── churn_prediction.ipynb
│   ├── clv_foundations.ipynb
│   └── survival_analysis.ipynb
│   └── clv_modelling.ipynb
├── outcome/               # Model outputs, results, or saved reports
└── README.md
