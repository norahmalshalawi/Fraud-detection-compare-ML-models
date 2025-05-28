
# Credit Card Fraud Detection

This project explores the use of supervised machine learning models to detect fraudulent transactions using real-world data. We evaluated and compared four classification models — Random Forest, Decision Tree, Logistic Regression, and Linear SVM — to determine the most effective approach for identifying credit card fraud.

> **Note:** This repository shares results and findings only. Source code is not included. For full details, see the [presentation](AML_presentation.pdf).

## Problem Statement

Fraudulent credit card transactions pose a significant threat to financial institutions and customers alike. Traditional rule-based methods are often ineffective when dealing with high-volume, fast-changing data. In this project, we leverage machine learning to develop a more robust, data-driven solution.

## Dataset

- **Source:** [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Original Size:** 284,807 transactions (492 fraud cases)
- **Class Imbalance:** Fraud cases were only 0.172% of total transactions
- **Preprocessing:**
  - Applied PCA (already included in dataset)
  - **Balanced the dataset** by randomly under-sampling the majority (non-fraud) class to match the number of fraud cases
  - Final dataset used: 492 fraud + 492 normal = 984 transactions

## Methodology

1. **Data Splitting:**  
   - Training: 80%  
   - Testing: 20%

2. **Models Evaluated:**
   - Random Forest
   - Decision Tree
   - Logistic Regression
   - Linear SVM

3. **Evaluation Metrics:**
   - Accuracy
   - Precision
   - Recall
   - F1-Score

## Results

- **Best Model:** Random Forest
- **Why:** 
  - Achieved the highest accuracy, precision, recall, and F1-score
  - Balanced detection of fraud (recall) and minimization of false alarms (precision)
  - Handles high-dimensional data and complex patterns effectively

## Analysis Summary

| Model              | Accuracy | Precision | Recall | F1-Score | Notes                              |
|-------------------|----------|-----------|--------|----------|------------------------------------|
| Random Forest      | High     | High      | High   | High     | Best overall performer             |
| Decision Tree      | High     | Moderate  | Moderate | High   | Prone to overfitting               |
| Logistic Regression| Moderate | Moderate  | Low    | Low      | Fast and simple, but less accurate |
| Linear SVM         | Moderate | Moderate  | Low    | Low      | Similar to Logistic Regression     |

## Learning Outcomes & Reflections

Through this project, we gained valuable experience in practical machine learning applications:

- **Data Challenges:** We learned how to handle imbalanced data and the importance of fair evaluation metrics.
- **Model Understanding:** We explored the strengths and trade-offs between various models, especially in high-stakes domains like fraud detection.
- **Analytical Thinking:** Comparing models using multiple metrics deepened our understanding of model performance beyond accuracy alone.
- **Team Collaboration:** This group project enhanced our communication and project planning skills, especially during data analysis and presentation preparation.
- **Real-World Relevance:** Understanding the business impact of fraud and the role of machine learning in mitigating it made this project highly meaningful.

## Contributors

- Lina Ahmed Alamri – 443007671  
- Lama Abdulmohsen Alquraishi – 443007691  
- Norah Mislat Alshalawi – 443007689  
- Raghad Abdullah Alanazi – 443007658

## Resources

- **Dataset:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Presentation:** [AML_presentation.pdf](AML_presentation.pdf)  
- **Colab Notebook:** [Google Colab](https://colab.research.google.com/drive/12EsqYHfzYgZaUUWLNTWTroR_oQEXhc56?usp=sharing)
