# Formative 2 - Data Preprocessing Assignment for Machine Learning Pipeline

## **Group Members:**
-MAHAMAT AHAMAT -Adediwura Emmanuel -Henriette Cyiza -Sabir Walid Abdurahman

## **Assignment Overview**
This assignment focuses on preprocessing and enhancing real-world datasets to ensure they are machine-learning-ready. The objective is to augment, merge, and clean data while maintaining consistency and integrity in a machine-learning pipeline.

This project assesses our ability to:
- Handle missing values in datasets.
- Merge datasets using transitive properties across features.
- Engineer new features to enhance data quality.
- Apply CSV augmentation techniques.
- Ensure data consistency for machine learning models.

---

## **Project Structure**
This assignment is divided into three main parts:

### **Part 1: Data Augmentation on CSV Files**
**Objective:** Expand and enhance an existing dataset using data augmentation techniques.

#### **Tasks:**
1. **Load the Dataset:**
   - Use the provided `customer_transactions.csv` dataset containing customer IDs, transaction histories, and purchase behaviors.

2. **Data Cleaning & Handling Missing Values:**
   - Identify and handle missing values using:
     - Mean, Median, Mode Imputation.
     - Predictive modeling to fill in missing data.

3. **Data Augmentation Strategies:**
   - **Synthetic Data Generation:**
     - Apply random noise to numerical transaction values.
     - Use SMOTE or interpolation to balance the dataset.
   - **Feature Value Transformation:**
     - Apply log transformation to skewed data.
   - **Data Expansion:**
     - Generate new synthetic transactions based on existing customer behaviors.

4. **Export the Augmented Data:**
   - Save the cleaned and augmented dataset as `customer_transactions_augmented.csv`.

---

### **Part 2: Merging Datasets with Transitive Properties**
**Objective:** Merge datasets with shared but indirect relationships between entities.

#### **Datasets Used:**
- `customer_transactions_augmented.csv` (from Part 1)
- `customer_social_profiles.csv` (contains social media activity and purchase intent data)
- `id_mapping.csv` (provides mapping between `customer_id_legacy` and `customer_id_new`)

#### **Tasks:**
1. **Identify the Link Between Datasets:**
   - The `customer_transactions_augmented.csv` dataset contains:
     - Customer ID, Purchase History, Amount Spent.
   - The `customer_social_profiles.csv` dataset contains:
     - Social Media Activity, Purchase Interest Score.
   - The datasets use different ID systems and require `id_mapping.csv` for linking.

2. **Perform a Complex Merge:**
   - Use `id_mapping.csv` to map customer IDs between datasets.
   - Merge datasets based on transitive relationships.
   - Handle cases where one legacy ID maps to multiple new IDs.

3. **Feature Engineering & Transformation:**
   - Create a **Customer Engagement Score** based on transaction history and social media activity.
   - Engineer predictive behavioral features using:
     - Moving averages of transactions.
     - Time-based aggregation of purchases.
     - TF-IDF vectorization on customer reviews or social media comments.

4. **Export the Final Preprocessed Data:**
   - Save the final merged and feature-engineered dataset as `final_customer_data_[groupNumber].csv`.

---

### **Part 3: Data Consistency and Quality Checks**
**Objective:** Ensure that the final dataset is clean, structured, and ready for machine learning models.

#### **Tasks:**
1. **Data Integrity Checks:**
   - Check for duplicate entries and remove them.
   - Ensure all categorical values are correctly mapped.
   - Validate that all customer transactions have a corresponding social profile.

2. **Statistical Summarization:**
   - Generate descriptive statistics (`describe()`) for all numerical columns.
   - Visualize the distribution of transaction amounts before and after augmentation.

3. **Feature Selection for Machine Learning:**
   - Identify highly correlated features using a correlation heatmap.
   - Select the top 10 most important features using a feature selection algorithm.

4. **Final Data Export:**
   - Save the cleaned and optimized dataset as `final_dataset_ready_[groupNumber].csv`.

---


## **Expected Outcomes**
- A structured and clean dataset ready for machine learning models.
- Improved data consistency and feature engineering.
- Insights into customer purchase behaviors through merged social media data.

---

## **Contributions**
-MAHAMAT AHAMAT -Adediwura Emmanuel -Henriette Cyiza -Sabir Walid Abdurahman





