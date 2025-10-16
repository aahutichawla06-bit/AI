**Telecom Churn Prediction Project**

**Project Purpose**
This notebook predicts whether a telecom customer is likely to **churn (leave the company)** or **stay**.  
Predicting churn helps telecom operators take proactive steps to retain customers and improve overall satisfaction.

 **Colab Notebook Link**
Access the full notebook here:  
https://colab.research.google.com/drive/1kuZF9GEGEPDdZhEziGVF52nhK9EXrBz4?usp=sharing

**Dataset Description**
The dataset (AI_p.csv) includes:
1.Demographics: gender, senior citizen, partner, dependents  
2.Account Info: tenure, contract type, billing method  
3.Services: internet service, streaming TV, phone, etc.  
4.Target Variable:`Churn` (Yes / No)

Each record represents one customer.


**Project Workflow**

 1️⃣ Data Preprocessing
Checked for missing values and handled them.  
Converted categorical columns to numerical using **Label Encoding**.  
Ensured dataset was clean and model-ready.

2️⃣ Splitting the Data
Data was divided into:
Training set (80%)** for model training  
Testing set (20%)** for evaluation  

3️⃣ Model Training
Three machine learning models were used:
Logistic Regression
Random Forest Classifier
LightGBM Classifier

4️⃣ Model Evaluation
Models were evaluated using:
Accuracy
Precision
Recall
F1-Score
Confusion Matrix



## Model Performance (Actual Results)

| Model | Precision (0) | Recall (0) | F1 (0) | Precision (1) | Recall (1) | F1 (1) | Key Insight |
|--------|---------------|------------|--------|----------------|------------|--------|--------------|
| **Logistic Regression** | 0.87 | 0.92 | 0.89 | 0.68 | 0.54 | 0.60 | Good precision on non-churn; moderate recall on churn |
| **Random Forest** | 0.84 | 0.93 | 0.88 | 0.67 | 0.44 | 0.53 | Very accurate for non-churn; needs improvement on churn detection |
| **LightGBM** | 0.89 | 0.83 | 0.86 | 0.56 | 0.67 | 0.61 | Balanced trade-off between precision and recall |

---

## Tools & Libraries Used
- **Python 3.x**
- **Pandas, NumPy** → Data processing  
- **Scikit-learn** → Model building and evaluation  
- **LightGBM** → Gradient boosting classifier  
- **Matplotlib, Seaborn** → Data visualization  

---

##  How to Run
1. Open the [Google Colab Notebook](https://colab.research.google.com/drive/1kuZF9GEGEPDdZhEziGVF52nhK9EXrBz4?usp=sharing)

2. Upload the dataset file (`AI_p.csv`)  
3. Run each cell sequentially  
4. Review model metrics and comparison table  

---

##  Insights & Interpretation
- Logistic Regression performs consistently with strong precision on non-churn customers.  
- Random Forest achieves the highest recall for non-churn but struggles slightly with churn detection.  
- LightGBM offers a more balanced performance, making it suitable when both precision and recall are important.  

---

##  Author
Tiet students
Data Science & Machine Learning Enthusiast  

