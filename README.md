# SCT_DS_TASK3
🧠 Task 3: Decision Tree Classifier for Customer Purchase Prediction

Task Objective:
Build a decision tree classifier to predict whether a customer will purchase a product or service based on their demographic and behavioral data. The dataset used for this task is the Bank Marketing dataset from the UCI Machine Learning Repository.

📌 Problem Statement
The goal is to develop a classification model that can predict customer response (yes or no) to a marketing campaign for a term deposit based on various customer features such as age, job, marital status, education, contact method, campaign history, etc.

🗃️ Dataset Description
•Source: UCI Machine Learning Repository

•File Used: bank-full.csv

•Target Variable: y – whether the client subscribed to a term deposit

•Type of Data: Demographic and behavioral features from marketing campaigns

Key Features:

•age, job, marital, education, default, balance, housing, loan

•contact, day, month, duration, campaign, pdays, previous, poutcome

🧪 Steps Performed

1.Data Preparation

•Loaded the dataset from bank-full.csv

•Explored the structure, checked data types, and verified missing values

•Label encoded the target variable (y)

•Applied one-hot encoding to categorical variables

2.Exploratory Data Analysis

•Visualized class distribution using bar charts

•Analyzed correlation between numerical variables

3.Model Building

•Trained multiple decision tree models using DecisionTreeClassifier:

•A default decision tree

•A pruned tree with constraints (max_depth, min_samples_leaf)

•A model excluding the duration column (to simulate real-time prediction use-case)

4.Model Evaluation

•Evaluated models using accuracy, confusion matrix, and classification report

•Compared model performance on training vs. test sets

•Visualized decision trees using plot_tree() from sklearn.tree

📊 Key Insights for Data Analysts

•The target variable (y) is highly imbalanced (majority "no" responses).

•Features like poutcome, previous, and contact played a significant role in prediction.

•Removing duration slightly impacted performance, confirming it's a post-call outcome and not useful for real-time prediction.

•Pruned decision trees offer a better generalization compared to fully grown ones.

📚 Libraries & Tools Used

•Python

•Pandas, NumPy

•Matplotlib, Seaborn

•Scikit-learn

✅ Outcome

Successfully built interpretable decision tree models that classify customer responses to marketing campaigns. The task demonstrated how customer data can be used to support decision-making in targeting strategies.
