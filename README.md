# Customer Churn Prediction (Machine Learning)
An end-to-end predictive machine learning project that identifies high-risk software subscribers before they cancel their subscriptions, enabling data-driven customer retention workflows.

![Live Prediction Output](prediction_output.png)

## 🛠️ Tech Stack & Skills Demonstrated
* **Python (Pandas, NumPy):** Data ingestion, median imputation for missing usage values, and categorical data mapping.
* **Scikit-Learn:** Random Forest Classifier execution, train-test splitting (stratified), and model performance reporting.
* **Matplotlib & Seaborn:** Behavioral feature visualization and density trend analysis.

## 📈 Project Pipeline

### 1. Data Cleaning & Engineering
* Handled missing values in account usage statistics using median imputation to stabilize model inputs.
* Converted nominal contract tracking fields into numerical data structures via custom mapping matrices.
* Dropped non-predictive administrative identifiers (`CustomerID`) to streamline operational feature sets.

### 2. Model Training & Evaluation
* Implemented a **Random Forest Classifier** consisting of 100 decision trees to reverse-engineer underlying behavioral trends.
* Split historical records into an 80/20 train-test layout, ensuring stratified target variable balances.
* Generated clear classification metrics (Precision, Recall, F1-Score) along with a confusion matrix to verify evaluation consistency.

### 3. Production Inference Design
* Developed an end-to-end simulation function allowing live customer usage matrices (tenure, contract type, tickets, activity hours) to run directly through the model pipeline.
* Configured the output to deliver a live binary decision alongside a specific percentage probability score to support prioritized target marketing.

## 📂 File Structure
* `Customer_Churn_Prediction.ipynb` - Complete Jupyter Notebook containing EDA, preprocessing, and model execution.
* `Software_Churn_Dataset.xlsx` - Formatted customer behavioral base data.
