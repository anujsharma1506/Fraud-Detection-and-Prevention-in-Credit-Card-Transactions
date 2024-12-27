# Fraud-Detection-and-Prevention-in-Credit-Card-Transactions

## Problem Statement  
The goal of this project is to predict fraudulent credit card transactions using machine learning models. By analyzing customer-level data from a collaborative research initiative between Worldline and the Machine Learning Group, this project identifies patterns in fraudulent behavior. The dataset, sourced from Kaggle, contains 284,807 transactions, of which only 492 are fraudulent. The highly imbalanced nature of the dataset necessitates specialized handling techniques to ensure the effectiveness of the predictive models.

---

## Problem Overview  
Credit card fraud significantly impacts banks and customers, leading to financial losses, eroded trust, and reduced credibility. For banks, retaining high-value customers while minimizing fraud is crucial. According to the Nilson Report, banking fraud was projected to reach $30 billion worldwide by 2020, driven by the growth of digital payment systems. The increasing sophistication of fraudulent schemes further exacerbates this challenge.  

Machine learning is essential for implementing proactive fraud prevention mechanisms, reducing manual review times, minimizing chargebacks, and enhancing customer satisfaction by avoiding false transaction denials.

---

## What is Fraud ?  
Credit card fraud encompasses unauthorized activities intended to extract financial gain from a cardholder's account. Common types of fraud include:  
- **Skimming**: Copying data from a card's magnetic strip.  
- **Card Manipulation**: Altering or forging legitimate cards.  
- **Counterfeit Cards**: Creating fake cards to mimic genuine ones.  
- **Lost/Stolen Cards**: Using misplaced or stolen credit cards for unauthorized transactions.  
- **Telemarketing Scams**: Exploiting cardholders through fraudulent phone calls.  

---

## Dataset Description  
The dataset includes two days of credit card transactions by European cardholders in September 2013. Out of 284,807 transactions, 492 are labeled as fraudulent, representing only 0.172% of the dataset.  

### Key Features:  
- **Time**: Elapsed time (in seconds) between the first and subsequent transactions.  
- **Amount**: Transaction amount.  
- **Class**: Binary label, where `1` represents fraudulent transactions and `0` represents legitimate ones.  

Principal Component Analysis (PCA) was applied to most features (`V1` to `V28`) to maintain confidentiality.

---

## Project Goals  
- Build a robust machine learning pipeline to accurately identify fraudulent transactions.  
- Improve performance on the minority (fraudulent) class using resampling techniques.  
- Ensure scalability and applicability in real-world scenarios.  

---

## Project Pipeline  

1. **Data Understanding**:  
   - Explore the dataset to understand its structure and relationships between features.  

2. **Exploratory Data Analysis (EDA)**:  
   - Conduct univariate and bivariate analyses.  
   - Address data skewness for optimal performance during model training.  

3. **Data Preprocessing**:  
   - Handle imbalanced data using SMOTE or undersampling techniques.  
   - Apply feature scaling, transformations, and encoding as needed.  

4. **Train/Test Split**:  
   - Perform stratified train-test splits for fair representation of the minority class.  
   - Use k-fold cross-validation for reliable evaluation.  

5. **Model Building**:  
   - Experiment with algorithms like Logistic Regression, Random Forest, and XGBoost.  
   - Optimize hyperparameters to enhance predictive accuracy.  

6. **Model Evaluation**:  
   - Use metrics like Precision, Recall, F1-Score, and AUC to prioritize fraud detection.  

---

## Key Challenges Addressed  
1. **Imbalanced Dataset**:  
   - Addressed through advanced resampling techniques.  
2. **False Positives**:  
   - Reduced to ensure legitimate transactions are not flagged unnecessarily.  
3. **Scalability**:  
   - Designed to handle large datasets and evolving fraud patterns.  

---

## Impact and Future Scope  

### Impact:  
- Reduces financial losses for banks.  
- Enhances customer trust and satisfaction.  
- Streamlines fraud detection processes.  

### Future Scope:  
- Integrating real-time detection systems.  
- Adapting to new fraud techniques.  
- Incorporating additional data sources for improved accuracy.  

