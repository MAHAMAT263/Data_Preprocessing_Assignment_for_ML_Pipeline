# Formative 2 - Data Preprocessing Assignment for Machine Learning Pipeline

## **Assignment Overview**
This assignment focuses on preprocessing and enhancing real-world datasets to ensure they are machine-learning-ready. The objective is to augment, merge, and clean data while maintaining consistency and integrity in a machine-learning pipeline.

This project assesses our ability to:
- Handle missing values in datasets.
- Merge datasets using transitive properties across features.
- Engineer new features to enhance data quality.
- Apply CSV augmentation techniques.
- Ensure data consistency for machine learning models.

---

## **Team Members and Contributions**
- Henriette Cyiza: Handled Part 1 - Data Augmentation (cleaning and expanding customer_transactions.csv).
- Mahamat Ahmat: Managed Part 2 - Merging Datasets (linking transactions and social profiles).
- Adedigba Adediwura: Took on Part 3 - Data Consistency and Quality Checks (ensuring the final dataset is ML-ready).

---

## **Repository Structure**

Formative2-Group[Number]/
├── Notebook/
│   ├── preprocessing_notebook.ipynb  <br/>
│   ├── customer_transactions.csv     <br/>
│   ├── customer_social_profiles.csv  <br/>
│   ├── id_mapping.csv                <br/>
│   ├── customer_transactions_augmented.csv  <br/>
│   ├── final_customer_data_[groupNumber].csv  <br/>
│   └── final_dataset_ready_[groupNumber].csv  <br/>
├── Models/  <br/>
│   └── spending_prediction_model.pkl  <br/>
├── report.pdf  <br/>
├── video_presentation.mp4  <br/>
└── README.md  <br/>

---

## **How to Set Up and Run**

### **Prerequisite**
Python 3.8+  <br/>
Libraries: Install via pip install -r requirements.txt or manually:  <br/>
- pandas  <br/>
- numpy  <br/>
- scikit-learn (for SMOTE and feature selection)  <br/>
- matplotlib and seaborn (for visualizations)  <br/>
- A Jupyter Notebook environment (e.g., JupyterLab, VS Code) <br/>

### **Steps**
1. Clone the repository
2. Install Dependencies
3. Run the Notebook
4. View Outputs

---

## **Project Details**

### **Part 1: Data Augmentation**
- Input: customer_transactions.csv (columns: transaction_id, amount_spent, purchase_date, etc.)
- Tasks: Cleaned missing values, added random noise to amount_spent, and created synthetic rows.
- Output: customer_transactions_augmented.csv

### **Part 2: Merging Datasets**
- Inputs: customer_transactions_augmented.csv, customer_social_profiles.csv (columns: social_media_platform, engagement_score), id_mapping.csv
- Tasks: Merged using id_mapping.csv, added features like customer_engagement_score and transaction_moving_avg.
- Output: final_customer_data_[groupNumber].csv (uploaded)

### **Part 3: Data Consistency and Quality Checks**
- Input: final_customer_data_[groupNumber].csv
- Tasks: Checked repeats in transaction_id, verified product_category and social_media_platform, analyzed amount_spent and customer_rating, selected top features (e.g., amount_spent, engagement_score), and exported final_dataset_ready_[groupNumber].csv.
- Output: final_dataset_ready_[groupNumber].csv

### **Bonus Challenge**
- Trained a model to predict amount_spent, saved in Models/.

---

## **Expected Outcomes**
- A structured and clean dataset ready for machine learning models.
- Improved data consistency and feature engineering.
- Insights into customer purchase behaviors through merged social media data.

---

## **Key Files**
- report.pdf (One-page summary of steps and insights.): https://docs.google.com/document/d/1LbHbCj7qk9ohlcgGcPlvm_mRnHJf1sn6ntAEwmALP0E/edit?usp=sharing
- video_presentation.mp4: https://drive.google.com/file/d/1WUPsZo2qEQBJtbxUvmldjcVH18XmEKKM/view?usp=sharing

---

## **Citations**
- Used pandas documentation for data handling [1].
- Referenced scikit-learn for SMOTE and feature selection [2].

[1] Pandas Development Team, Pandas Documentation, 2023. [Online]. Available: https://pandas.pydata.org/docs/

[2] Scikit-learn Developers, Scikit-learn User Guide, 2023. [Online]. Available: https://scikit-learn.org/stable/user_guide.html

---

## **Contributions**
-MAHAMAT AHAMAT -Adediwura Emmanuel -Henriette Cyiza -Sabir Walid Abdurahman





