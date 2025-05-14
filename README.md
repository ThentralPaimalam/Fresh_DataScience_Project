#  Student Performance Prediction - End-to-End Data Science Project
*COMPANY*: CODETECH IT SOLUTIONS

*NAME*: THENTRAL S

*INTERN ID*: CT08WN69

*DOMAIN*: DATA SCIENCE

*DURATION*: 8 WEEKS

*MENTOR*: NEELA SANTOSH
## Description
This project is an end-to-end implementation of a machine learning pipeline to predict student performance based on socio-economic and academic features. The purpose is to understand which factors impact students' scores and build a reliable model that can predict academic outcomes with high accuracy.


**Objective**

The goal of this project is to:

Predict student exam scores based on various features such as gender, lunch type, parental education, and test preparation.
Analyze the relationships and influence of input features on students’ academic performance.
Build a clean, reusable, and deployable machine learning pipeline.


## Dataset Description

The dataset contains information about student demographics and their scores in three subjects: math, reading, and writing.

**Key Features:**

- `gender`
- `race/ethnicity`
- `parental level of education`
- `lunch`
- `test preparation course`
- `math score`
- `reading score`
- `writing score`

The dataset was sourced from a public domain (UCI or Kaggle) and manually cleaned for use in this project.

 **Exploratory Data Analysis (EDA)**

Performed an in-depth exploratory data analysis to understand trends and relationships:

Visualized score distributions across demographic categories
Checked correlations among the three subject scores
Identified outliers and data skewness
Explored impact of parental education and test preparation on scores

Tools used: `Pandas`, `Matplotlib`, `Seaborn`


**Data Preprocessing**

Key preprocessing steps:

Handled categorical variables using OneHotEncoding
Scaled numerical features using `StandardScaler`
Split data into train/test (80/20)
Ensured consistency in preprocessing using `ColumnTransformer` and `Pipeline`


**Model Building & Evaluation**

Trained multiple regression models:

- Linear Regression
- Ridge and Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- CatBoost Regressor

After evaluation using metrics like R² Score, MAE, and RMSE, **CatBoost Regressor** was selected as the final model due to its superior accuracy and performance with categorical variables.


**Evaluation Metrics**

- **R² Score**: Measures the proportion of variance explained
- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **Cross-Validation Score (10-fold)**

The CatBoost model achieved an R² score of over **94%**, indicating strong predictive capability.

**Model Saving & Deployment Preparation**

- The final model and preprocessing pipeline were saved using `joblib`
- Flask-based structure prepared for easy deployment
- The project can be turned into a web app where users input student details and receive predicted scores


## Output

![Image](https://github.com/user-attachments/assets/5686c563-6d1f-4eb8-82cb-d9649524e03e)

