
# Ecommerce Data Analysis and Churn Prediction  
📊 **Understanding and Addressing Customer Churn in E-commerce**

---

## **Overview**  
This project focuses on analyzing e-commerce customer data to predict churn and derive actionable insights. By leveraging data preprocessing, exploratory analysis, feature engineering, and machine learning, it provides a structured approach to understanding customer behavior and the factors contributing to churn.

---

## **Dataset**  
The dataset includes key information:  
- **Demographics**: Age group, gender, subscription tenure.  
- **Transaction Data**: Monthly spend, total spend, and frequency of purchases.  
- **Churn Status**: A binary indicator of whether a customer has stopped purchasing.  

> **Note**: Due to licensing restrictions, raw data is not included. Instructions to download and use the dataset are available in the `data/` folder.

---

## **Project Workflow**  
The project is structured into four major steps, each detailed in separate Jupyter notebooks.

---

### **Step 1: Data Cleaning**  
**Objective**: Prepare the raw data for analysis by addressing issues like missing values, duplicates, and incorrect data types.  

**What’s in the notebook**:  
- Loading the raw dataset (`dataset.csv`).  
- Removing duplicates and handling missing values.  
- Verifying data consistency and integrity.  

**File**: `01_data_cleaning.ipynb`  
**Output**: `cleaned_dataset.csv`

---

### **Step 2: Exploratory Data Analysis (EDA)**  
**Objective**: Gain insights into customer behavior and transaction trends using visualizations and statistics.  

**What’s in the notebook**:  
- Analyzing customer demographics (e.g., age group distribution).  
- Identifying trends in purchase frequency, spend, and engagement.  
- Exploring correlations between features and churn status.  

**File**: `02_eda.ipynb`  
**Output**: Visualizations saved in the `visuals/` folder.

---

### **Step 3: Feature Engineering**  
**Objective**: Create meaningful features to enhance model performance.  

**What’s in the notebook**:  
- Creating derived features like:  
  - **Customer Lifetime Value (CLV)** = Monthly Spend × Subscription Tenure.  
  - **Recency**: Days since the last purchase.  
  - **Engagement Level**: Categorized as High, Medium, or Low.  
- Encoding categorical variables (e.g., Engagement Level).  

**File**: `03_feature_engineering.ipynb`  
**Output**: `engineered_dataset.csv`

---

### **Step 4: Model Training and Evaluation**  
**Objective**: Build and evaluate a machine learning model to predict churn.  

**What’s in the notebook**:  
- Splitting the data into training and testing sets.  
- Training a **Random Forest Classifier** for churn prediction.  
- Evaluating the model using:  
  - Confusion Matrix.  
  - ROC-AUC Score.  
  - Visualizations of predictions and performance metrics.  

**File**: `04_model_training.ipynb`  

---

## **Directory Structure**  
```
📁 data/  
   ├── dataset.csv             # Raw dataset  
   ├── cleaned_dataset.csv     # Dataset after cleaning  
   ├── engineered_dataset.csv  # Dataset after feature engineering  

📁 notebooks/  
   ├── 01_data_cleaning.ipynb      # Data cleaning step  
   ├── 02_eda.ipynb                # Exploratory Data Analysis  
   ├── 03_feature_engineering.ipynb # Feature engineering step  
   ├── 04_model_training.ipynb     # Model training and evaluation  

📁 visuals/  
   # Folder for saved plots and visualizations from EDA and model evaluation  

📜 .gitignore           # Git ignore file for unnecessary files  
📜 LICENSE              # License for the project  
📜 README.md            # Project overview and instructions  
```

---

## **How to Run the Project**  
1. **Clone the repository**:  
   ```bash
   git clone https://github.com/jyothsnacreator/Ecommerce_Dataanalysis.git
   cd Ecommerce_Dataanalysis
   ```

2. **Set up your environment**:  
   ```bash
   python -m venv venv
   source venv/bin/activate  # Mac/Linux
   venv\Scripts\activate   # Windows
   ```

3. **Install required packages**:  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Jupyter notebooks**:  
   Execute the notebooks sequentially:
   ```bash
   jupyter notebook
   ```

---

## **Acknowledgments**  
This project uses an e-commerce dataset inspired by public sources like Kaggle. Special thanks to the contributors of such datasets.

---

## **License**  
This project is licensed under the Apache 2.0 License. See the `LICENSE` file for details.

