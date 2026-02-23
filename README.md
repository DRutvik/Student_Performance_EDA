# Student Performance Analysis

---

## Project Overview
This project analyzes student performance data to understand the factors that affect academic success. It explores relationships between demographics, study habits, parental background, and student scores, and builds machine learning models to predict average performance.  

The dataset includes information like gender, ethnic group, parental education, lunch type, test preparation, study hours, and exam scores.

---

## Project Objectives
- Explore student data to identify trends and patterns.  
- Clean, preprocess, and encode categorical features for machine learning.  
- Engineer features like total and average scores, and categorize performance levels.  
- Visualize key relationships using plots and heatmaps.  
- Train and compare machine learning models (Random Forest & XGBoost) to predict student performance.  
- Evaluate models with MAE, MSE, RMSE, and R² metrics.  
- Identify the most influential features using feature importance.

---

## Technologies Used
- **Python Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`  
- **Machine Learning:** `scikit-learn` (`RandomForestRegressor`, train-test split, evaluation metrics)  
- **Gradient Boosting:** `xgboost` (`XGBRegressor`, feature importance)  

---

## Dataset
The dataset `Expanded_data_with_more_features.csv` contains:

| Column | Description |
|--------|-------------|
| gender | Student's gender |
| ethnic_group | Student's ethnic background |
| parent_education | Highest level of parental education |
| lunch_type | Type of lunch (standard / free/reduced) |
| test_prep | Completion of test preparation course (yes/no) |
| parent_marital_status | Marital status of parents |
| practice_sport | Whether student practices sports |
| is_first_child | Whether student is the first child |
| no_of_siblings | Number of siblings |
| transport_means | Means of transport to school |
| weekly_study_hours | Weekly study hours category (<5, 5-10, >10) |
| math_score | Score in math exam |
| reading_score | Score in reading exam |
| writing_score | Score in writing exam |

**Engineered Features:**  
- `total_score`: Sum of math, reading, and writing scores  
- `avg_score`: Average of the three scores  
- `performance_level`: Low / Medium / High based on average score  
- `weekly_study_hours_num`: Numeric conversion of study hours  

---

## Project Workflow

### 1. Data Preprocessing
- Drop unnecessary columns  
- Fill missing values  
- Rename columns for clarity  

### 2. Feature Engineering
- Total and average scores  
- Categorized performance levels  
- Convert study hours from categorical to numeric  

### 3. Data Visualization
- Countplots, boxplots, heatmaps, pie charts  
- Pivot tables for study hours & test prep interaction  

### 4. Encoding
- Convert categorical features to numeric using `LabelEncoder`  

### 5. Train-Test Split
- 80% training, 20% testing to evaluate model performance fairly  

### 6. Machine Learning Models
- **Random Forest Regressor** (non-linear relationships)  
- **XGBoost Regressor** (gradient boosting for accuracy)  

### 7. Model Evaluation
- Metrics: MAE, MSE, RMSE, R²  
- Compare performance between Random Forest and XGBoost  

### 8. Feature Importance
- Identify key factors affecting student performance  
- Important features: study hours, test prep, parental education  

