# Predicting-Employee-Attrition-Using-Logistic-Regression
Predicting Employee Attrition Using Logistic Regression

**Definition:**

Logistic Regression is a statistical method for predicting binary outcomes (e.g., yes/no, 0/1) based on one or more independent variables. 
In the context of Employee Attrition Prediction, the binary outcome is whether an employee will leave the company (Attrition = 1) or stay (Attrition = 0).

**Reason behind Logistic regression (Why)**

Logistic Regression is particularly suited for binary classification tasks. 
Unlike Linear Regression, it outputs probabilities and uses the Sigmoid Function to map predictions between 0 and 1:

𝑃(Attrition=1)=1/1+𝑒−(𝛽0+𝛽1𝑥1+𝛽2𝑥2+⋯+𝛽𝑛𝑥𝑛)

Where:
P(Attrition=1) is the probability of an employee leaving.
𝛽0,𝛽1,…,𝛽𝑛 are model coefficients learned during training.
𝑥1,𝑥2,…,𝑥𝑛  are feature values (e.g., age, satisfaction level).

**Steps in the Logistic Regression Model**
**Data Preprocessing:**
Categorical variables (e.g., Gender, Department, Role) are encoded into numerical values.
Numerical variables (e.g., Work_Hours, Satisfaction_Level) are standardized to ensure features are on the same scale.

**Model Training:**
Logistic Regression learns the coefficients (𝛽) by maximizing the log-likelihood function. 
It adjusts the coefficients to minimize the difference between the predicted probabilities and the actual outcomes.

**Prediction:**
For a new employee record, the model predicts the probability of attrition.
If P(Attrition=1)>0.5, the employee is predicted to leave.
Otherwise, the employee is predicted to stay.

**Evaluation:**
Accuracy: Measures overall correctness of the model.

Precision: Focuses on correctly predicting employees who actually left.

Recall: Measures how well the model identifies actual attrition cases.

ROC-AUC: Evaluates the model's ability to separate churners from non-churners.

**Why Logistic Regression is Valuable in this Use Case**

**Simplicity:** Easy to implement and interpret, making it a good starting point for predicting attrition.

**Transparency:** Coefficients clearly explain the influence of features on attrition.

**Actionable Insights:** HR departments can focus on high-risk employees and design retention strategies.

**Scalability:** Works effectively for small to moderately large datasets commonly used in such predictions.

**Industry Context:**

**Amazon:** Predict whether employees will leave the company based on job satisfaction, workload, and growth opportunities.

**Meta:** Predict the likelihood of employee attrition due to work-life balance or job role alignment.

**NVIDIA:** Determine if high-performing engineers are at risk of leaving due to stress or lack of promotions.

**Walmart:** Predict whether hourly employees are likely to quit based on work hours and tenure.

**Netflix:** Identify employees likely to resign to proactively offer retention strategies.

