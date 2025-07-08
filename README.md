# 📊 Customer Churn Prediction using Apache Spark (PySpark)

This project demonstrates an **end-to-end machine learning pipeline** built using **Apache Spark (PySpark)**.  
We analyze customer behavior data to predict churn using a logistic regression model, combined with data cleaning, feature engineering, model tuning, and exporting final results.

---

## 🚀 Project Highlights

- Built entirely with **Apache Spark via PySpark**
- Handles **large-scale tabular data**
- End-to-end ML pipeline using **Spark MLlib**
- Includes:
  - Data cleaning
  - Feature engineering (indexing + assembling)
  - Model training using logistic regression
  - Cross-validation with hyperparameter tuning
  - Churn rate analysis by contract type
  - Saving outputs and model artifacts

---

## 🛠️ Technologies Used

- Apache Spark 3.x
- PySpark (DataFrame API + MLlib)
- Logistic Regression (binary classification)
- CrossValidator for model tuning
- Pandas/CSV output compatible with cloud or local processing

---

## 📁 Folder Structure / Output Explanation

After running the notebook, you will see two output folders:

### `/output/predictions/`
- Contains a file like:  
  `part-00000-<uuid>.csv`
- **Includes:** model predictions and churn probabilities for each customer.
- Columns:
  - `customerID`: Unique identifier
  - `prediction`: Churn prediction (0 = No, 1 = Yes)
  - `churn_probability`: Probability of churn (from logistic regression)

### `/output/churn_rate_by_contract/`
- Contains a file like:  
  `part-00000-<uuid>.csv`
- **Includes:** churn rate aggregated by contract type.
- Helps answer: *Which customer contracts have the highest churn rate?*

---

## 📦 How to Run

### 🔹 Option 1: On Google Colab (Recommended for Beginners)

1. Upload this notebook to Colab
2. Upload your dataset (e.g., `customer_churn.csv`)
3. Install PySpark:
   ```bash
   !pip install pyspark
Run all cells

🔹 Option 2: Locally
Install Spark:

bash
Copy
Edit
pip install pyspark
Run the script in Jupyter Notebook or any Python environment

📈 Sample Output Screenshot
(Optional: Add image of churn_rate_by_contract or prediction DataFrame)

📘 Dataset Used
Telco Customer Churn Dataset
🔗 Kaggle [Link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

📄 License
MIT License © 2025 Arjun Jagdale
