# Data-Analyzer
# 🏥 Ubuntu General Hospital — Data Analysis & AI Predictions

*"I am because we are"* — This project simulates a hospital’s patient dataset and applies **data science + machine learning** to explore, clean, visualize, and predict patient needs. Inspired by **Ubuntu principles**, the work emphasizes collective care, balance, and meaningful insights.

---

## 📂 Project Structure

ubuntu-hospital-analysis/
│── ubuntu_analysis.py # Main Python script with full workflow

yaml
Copy code

---

## 🚀 Features

### 🔎 Data Simulation & Exploration
- Generates a dataset of **100 patients** with:
  - `Patient_ID`
  - `Age`
  - `Gender`
  - `Condition` (Flu, Diabetes, Hypertension, Asthma, Healthy)
  - `Treatment Duration (Days)`
  - `Satisfaction Score` (1–10 scale)
  - `Follow_Up_Needed` (True/False)

- Displays:
  - First 10 patients  
  - Average age, most common condition  
  - Gender distribution  
  - Satisfaction statistics  

---

### 🧹 Data Cleaning
- Introduces **missing values** in `Satisfaction_Score`.
- Fills gaps with **community average score** (Ubuntu principle: *no one left behind*).  

---

### 📊 Visualizations
- **Condition Distribution** (countplot)
- **Treatment Duration by Condition** (boxplot)
- **Satisfaction vs Treatment Duration** (scatterplot, colored by condition)
- **Confusion Matrix** (ML performance evaluation)

---

### 🤖 Machine Learning
- Prepares dataset with **one-hot encoding** for categorical variables.  
- Splits into **training & test sets**.  
- Trains a **Random Forest Classifier** to predict:
  - `Follow_Up_Needed` (Yes/No).  
- Outputs:
  - **Classification report** (precision, recall, F1-score).  
  - **Confusion matrix** heatmap.  

---

## 📦 Requirements

Install required libraries before running:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
▶️ How to Run
Clone this repository or copy the script into VS Code.

Save the file as ubuntu_analysis.py.

Run the script:

bash
Copy code
python ubuntu_analysis.py
✅ You will see:

Patient statistics in the terminal.

Multiple visualizations opening in windows.

Machine learning results in the terminal and confusion matrix plot.

📊 Example Insights
Most common conditions often include Flu and Diabetes.

Asthma patients typically need longer treatments.

Satisfaction has a slight negative correlation with treatment duration (longer stays → slightly lower scores).

Random Forest Model predicts follow-up needs with reasonable accuracy.

🌍 Ubuntu Principles in Action
Community Care → Missing values filled with collective average.

Compassionate Analytics → Visuals help understand shared health burdens.

Preparedness → Predicting follow-up needs enables proactive care.

Beyond Metrics → Reflections added to see meaning, not just numbers.

💡 Next Steps
Try with real datasets (e.g., Kaggle’s Heart Disease UCI or Diabetes Health Indicators).

Add more advanced models (XGBoost, Neural Networks).

Deploy as a Flask/Django web app for interactive use.

Share results with others — learning grows when shared.

👨‍💻 Author
Penuel Isaac
Data Enthusiast | Machine Learning Explorer | Ubuntu Believer
