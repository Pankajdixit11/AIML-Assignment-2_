# Customer Churn Prediction using Logistic Regression

## Objective:
A telecommunications company wants to predict whether a customer is likely to leave (churn) based on demographic information and service usage. 
Develop a Logistic Regression model to predict customer churn.

## Dataset

Source: [Telco Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

Dataset Statistics:
-Total Records: 7,043 customers
-Total Features: 21 columns
-Target Variable: Churn (Yes/No)
-Churn Rate: ~26.5%

## Assignment Tasks
Task 1: Data Understanding (2 Marks)
- Load the dataset using Pandas
- Display first five records
- Identify numerical features, categorical features, and target variable

Task 2: Data Preprocessing (2 Marks)
- Check for missing values
- Handle missing values (TotalCharges column conversion)
- Encode categorical variables using LabelEncoder
- Split dataset (80% training, 20% testing)
- Feature scaling using StandardScaler

Task 3: Model Development (3 Marks)
- Build Logistic Regression model
- Train the model on training data
- Predict customer churn on test dataset
- Extract feature importance coefficients

Task 4: Model Evaluation (2 Marks)
- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix with visualization
- Model performance observations

Task 5: Conclusion (1 Mark)
- Key findings
- Factors influencing customer churn
- Limitations of Logistic Regression
- Business recommendations

## Model Performance
Evaluation Metrics:
| Metric	| Score |
|---|---|
| Accuracy	| ~80% |
| Precision	| ~0.63 |
| Recall	| ~0.54 |
| F1-Score	| ~0.58 |

![Confusion Matrix](https://github.com/Pankajdixit11/AIML-Assignment-2_/blob/7286394fbfa4ba7aa608aabcff442afe460df0f5/churn_analysis_results.png)

#Key Performance Insights
- Accuracy: The model achieves ~80% accuracy, significantly better than random guessing (73.5% baseline)
- Precision-Recall Trade-off: The model has better precision than recall, meaning it's more conservative in predicting churn
- Confusion Matrix Analysis:
- Correctly identifies ~54% of actual churners
- Has moderate false positive rate

**Visualizations**
- The project generates several visualizations:
- Confusion Matrix Heatmap - Shows prediction accuracy breakdown
- Feature Importance Plot - Top 10 features affecting churn
- Model Performance Dashboard - Comprehensive metrics visualization

**Limitations**
- Linearity Assumption: Logistic Regression assumes linear relationships between features and log-odds
- Feature Independence: Cannot capture complex feature interactions
- Class Imbalance: Dataset has ~26.5% churn rate, causing bias toward non-churn predictions
- Non-linear Relationships: Cannot capture complex patterns in customer behavior

**References:**
- [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Logistic Regression Theory](https://en.wikipedia.org/wiki/Logistic_regression)

**License:** This project is for educational purposes. The dataset is provided by IBM and is available for public use.

**Contributor:**
- Pankaj Dixit

**Acknowledgments**
- IBM for providing the dataset
- Kaggle for hosting the dataset
- Open-source community for excellent libraries

##CONCLUSION
- Key Findings: The Logistic Regression model achieved {accuracy*100:.2f}% accuracy in predicting customer churn, with contract type, tenure, and monthly charges as the strongest predictors.
