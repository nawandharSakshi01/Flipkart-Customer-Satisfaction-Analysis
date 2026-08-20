# Customer Support Query Analysis & CSAT Prediction

## 📌 Project Overview

This project analyzes customer support interactions to understand customer issues, communication channels, product categories, handling time, and customer satisfaction.

The project also prepares the customer support data for Machine Learning to predict **Customer Satisfaction (CSAT) Scores** based on customer interaction and support-related features.

## 🎯 Objectives

* Analyze customer support queries and their patterns.
* Understand customer satisfaction across different categories and channels.
* Identify important factors affecting CSAT scores.
* Perform data cleaning and preprocessing.
* Apply Natural Language Processing (NLP) techniques to customer remarks.
* Create meaningful features from date-time information.
* Prepare the dataset for Machine Learning.
* Build a model to predict CSAT scores.

## 📊 Dataset

The dataset contains **85,907 customer support interactions** with information related to:

* Communication channel
* Customer issue category
* Sub-category
* Product category
* Customer city
* Item price
* Handling time
* Agent information
* Agent shift
* Agent tenure
* Customer remarks
* CSAT Score
* Response time

## 🔍 Exploratory Data Analysis

The following analyses and visualizations were performed:

* Overall Customer Support Query Analysis
* Product Category Distribution
* Customer Queries by Communication Channel
* Customer Issue Category Distribution
* Customer Satisfaction Score Distribution
* Customer Queries by Sub-category
* Top 10 Customer Cities
* Average Handling Time by Agent Shift
* Average CSAT Score by Agent Shift
* Average CSAT Score by Agent Tenure
* Product Category vs CSAT Score
* Item Price vs CSAT Score
* Communication Channel vs Issue Category
* Category and Channel vs CSAT Score
* Agent Shift and Channel vs CSAT Score
* Pair Plot of Numerical Variables
* Correlation Heatmap

## 🧹 Data Preprocessing

The following preprocessing techniques were applied:

* Missing value detection
* Missing value imputation
* Duplicate removal
* Outlier detection using the IQR method
* Outlier capping
* Removal of unnecessary identifier columns
* Categorical feature encoding using One-Hot Encoding
* Feature scaling using StandardScaler
* Train-test splitting

## 📝 Natural Language Processing

Customer remarks were processed using several NLP techniques:

* Contraction expansion
* Lowercasing
* Punctuation removal
* URL removal
* Removal of words containing digits
* Stopword removal
* Whitespace removal
* Tokenization
* Lemmatization
* Part-of-Speech (POS) tagging
* TF-IDF vectorization

## ⚙️ Feature Engineering

New features were created from date-time information:

* Order Hour
* Order Day
* Order Month
* Order Day of Week
* Response Time in Hours

These features help identify time-based patterns in customer support interactions.

## 🎯 Feature Selection

Unnecessary features such as unique identifiers, order IDs, raw date-time columns, and raw customer remarks were removed to reduce unnecessary model complexity and avoid overfitting.

## 🤖 Machine Learning

The target variable for Machine Learning is:

**CSAT Score**

The dataset was divided into:

* **80% Training Data**
* **20% Testing Data**

The CSAT target was found to be imbalanced, with CSAT Score 5 representing the majority of observations. Therefore, class balancing techniques such as `class_weight='balanced'` can be used during model training.

### ML Model 1: Logistic Regression

Logistic Regression was selected as the first classification model because CSAT Score represents discrete classes.

The model is evaluated using classification metrics such as:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

## 📈 Results

The Machine Learning model is evaluated on the test dataset using classification evaluation metrics.

The final model performance and evaluation charts will be added after completing model training and testing.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* NLTK
* SciPy
* Jupyter Notebook
* GitHub

## 📁 Project Structure

```text
Customer-Support-Query-Analysis/
│
├── Customer_support_data.csv
├── Customer_Support_Query_Analysis.ipynb
├── README.md
└── requirements.txt
```

## ▶️ How to Run

1. Clone the repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Place the dataset in the project directory.
5. Run the notebook cells sequentially.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk scipy
```

## 👩‍💻 Author

**Sakshi Nawandhar**

B.Tech – Computer Science Engineering
