# 🚗 Modeling Car Insurance Claim Outcomes

## 🏁 Project Goal
The primary objective of this project is to identify the best predictors of whether a customer will make a car insurance claim using logistic regression. By analyzing client demographic, vehicle, and behavioral data, we aim to:
- Predict claim outcomes with high accuracy.
- Understand the relative importance of various features in influencing claim likelihood.

---

## 🔍 Dataset Description
The dataset includes information about car insurance clients and contains the following key features:
- **Demographics**: Age, Gender, Marital Status, Education, Income Level.
- **Vehicle Information**: Ownership status, Year of Registration, Type of Vehicle.
- **Behavioral Data**: Driving experience, Annual mileage, Past accidents, Speeding violations, DUIs.
- **Target Variable**: `outcome` (0 = No claim, 1 = Made a claim).

The dataset has been preprocessed to ensure it is suitable for modeling, with all missing values handled appropriately.

---

## 🛠️ Methodology
1. **Data Preprocessing**:
   - Identified and handled missing values using imputation techniques.
   - Retained categorical features as integers (no additional encoding).

2. **Modeling**:
   - Logistic regression was chosen for its interpretability and effectiveness in binary classification problems.
   - Splitted the dataset into training (70%) and testing (30%) sets.
   - Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score.

3. **Feature Importance Analysis**:
   - Examined the coefficients of the logistic regression model to understand the importance of different predictors.

---

## 📊 Key Outcomes
### 1. **Model Performance**
- **Accuracy**: 84.77%
- **Classification Report**:
  | Metric       | Class 0 (No Claim) | Class 1 (Made a Claim) | Overall |
  |--------------|--------------------|------------------------|---------|
  | Precision    | 0.88               | 0.77                   | -       |
  | Recall       | 0.90               | 0.73                   | -       |
  | F1-score     | 0.89               | 0.75                   | -       |
  | Weighted Avg | -                  | -                      | 0.85    |

### 2. **Feature Importance**
The table below shows the features most influential in predicting claim outcomes:
| Feature                      | Importance |
|------------------------------|------------|
| Driving Experience (30+ years) | 3.54       |
| Driving Experience (20-29 years) | 2.98     |
| Vehicle Year (Before 2015)    | 1.64       |
| Vehicle Ownership             | 1.64       |
| Driving Experience (10-19 years) | 1.62    |
| Gender (Male)                 | 0.95       |
| Past Accidents                | 0.44       |
| Marital Status (Married)      | 0.41       |
| Speeding Violations           | 0.15       |
| Age Group (65+)               | 0.14       |

---

## 📈 Visualizations
1. **Distribution of Claims**:  
   - This bar chart shows the distribution of claim outcomes across all clients. It helps in understanding the overall proportion of clients making claims versus those who don't.
2. **Credit Score Distribution by Outcome**:  
   - This histogram shows the credit score distribution for both claim outcomes (No Claim and Made a Claim). It reveals any patterns or differences in credit scores between the two groups.
3. **Annual Mileage by Income Group and Claim Outcome**:  
   - This boxplot visualizes the relationship between income groups, annual mileage, and claim outcomes. It highlights trends and variations in mileage across different income levels and claim statuses.
4. **Feature Importance Chart**:
  - A bar plot showcasing the relative importance of features.
5. **Confusion Matrix**:
  - Visualization of true vs. predicted values to highlight model accuracy.

---

## 🧠 Conclusion
- The model achieved a strong **accuracy of 84.77%**, demonstrating reliable performance in predicting claim outcomes.
- **Driving experience** and **vehicle ownership** emerged as the most influential predictors of insurance claims.
- Opportunities for improvement include testing other machine learning models (e.g., decision trees or ensemble methods) and incorporating additional features for better prediction accuracy.

---

## 🛠️ Future Work
- Exploring other classification algorithms such as Random Forests or Gradient Boosting to compare performance.
- Performing hyperparameter tuning to optimize the logistic regression model.
- Developing a dashboard to visualize insights interactively.

---
## 🤝 Acknowledgements
- The dataset used in this project is sourced from [`https://www.accenture.com/_acnmedia/pdf-84/accenture-machine-leaning-insurance.pdf`].
- Special thanks to the Scikit-learn library for enabling effective model implementation.

---
## 📬 Contact
- **Project Author**: Binita Roy 
For questions or feedback, reach out to me at [LinkedIn](https://www.linkedin.com/in/binita-roy/) | [Email](mailto:binitaroy1312@gmail.com).
 


