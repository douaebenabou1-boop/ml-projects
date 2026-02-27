# ml-projects
Projects in Machine Learning and Data Science
#  Fraud Detection using Machine Learning  
## Comparative Analysis and Model Selection

---

## Project Objective

The objective of this project is to conduct a comparative study of multiple Machine Learning classification models to identify the most effective algorithm for fraud detection.

Rather than relying on a single model, this project evaluates and justifies the selection of the best-performing model based on robust evaluation metrics and performance analysis.

Fraud detection is a high-stakes classification problem where minimizing false negatives (undetected fraud) is critical.

---

## Dataset

The dataset contains financial transaction records labeled as:

- 0 → Legitimate transaction  
- 1 → Fraudulent transaction  

Due to the imbalanced nature of fraud detection data, evaluation metrics beyond simple accuracy were considered essential.

---

##  Technologies and Tools

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- StandardScaler  
- GridSearchCV  
- Jupyter Notebook  

---

##  Methodology

### 1️- Data Preprocessing
- Data cleaning  
- Feature scaling using StandardScaler  
- Train/Test split  
- Preparation for fair model comparison  

---

### 2️- Models Implemented and Compared

The following models were implemented and optimized:

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
  - Linear Kernel
  - Polynomial Kernel
  - RBF (Radial Basis Function) Kernel
- Decision Tree

Hyperparameter tuning was performed using GridSearchCV to ensure optimal performance for each model.

---

### 3️- Evaluation Metrics

Given the sensitivity of fraud detection, the following metrics were analyzed:

- Accuracy  
- Recall (Fraud Detection Rate)  
- F1-Score  
- Confusion Matrix  

Special emphasis was placed on Recall to reduce false negatives and ensure fraudulent transactions are detected effectively.

---

##  Results Summary

| Model              | Accuracy | Recall | Key Observation |
|--------------------|----------|--------|----------------|
| KNN (K=5)          | ~93.5%   | 47.6%  | Good at minimizing false positives |
| SVM Linear         | ~92.0%   | 40.0%  | Too rigid for complex fraud patterns |
| SVM Polynomial     | ~94.0%   | 75.0%  | Good capture of nonlinear relationships |
| **SVM RBF**        | **~94.2%** | **89.5%** | Best overall performance |
| Decision Tree      | ~91.0%   | 60.0%  | Interpretable but less stable |

---

## Final Model Selection

The **SVM with RBF kernel** was selected as the best-performing model because:

- It achieved the highest Recall (89.5%)
- It maintained strong overall Accuracy
- It provided the best balance between fraud detection and false positives
- It demonstrated robustness without overfitting

The RBF kernel allowed the model to capture complex nonlinear fraud patterns more effectively than linear or polynomial kernels.

---

##  Ethical Considerations

Fraud detection systems may raise concerns such as:

- Potential discrimination bias  
- Human impact due to false positives  
- Lack of transparency  

To address these risks, this project emphasizes AI as a **decision-support system**, where the final decision remains under human supervision.

---

## Skills Demonstrated

- Comparative model analysis  
- Hyperparameter optimization with GridSearchCV  
- Kernel selection in SVM  
- Handling imbalanced classification problems  
- Model evaluation and justification  
- Ethical considerations in AI systems  

---

##  Future Improvements

- Cross-validation  
- SMOTE or advanced imbalance handling techniques  
- Advanced ensemble methods (XGBoost, Gradient Boosting)  
- Deployment as a real-time fraud detection support tool  

---

##  Author

Douae Benabou  
Master in Artificial Intelligence & Data Science  
Machine Learning | Deep Learning | Python  
