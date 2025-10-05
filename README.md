# Cyber Security Assignment 2  
## Intrusion Detection System using Decision Tree

---

## Research Paper Reference
- **Title:** *Comparative Analysis of Intrusion Detection Systems and Machine Learning-Based Model Analysis Through Decision Tree*  
- **Source:** IEEE Xplore, 2023  
- **Link:** [https://ieeexplore.ieee.org/document/10185955](https://ieeexplore.ieee.org/document/10185955)  

This paper discusses various Machine Learning algorithms used for Intrusion Detection Systems (IDS), focusing on Decision Tree–based models.  
It highlights limitations such as outdated datasets, poor minority attack detection, and high false alarm rates.  

---

## Research Gap Identified
- Intrusion Detection Systems often rely on outdated datasets (KDD, NSL-KDD) that do not represent modern cyber attacks.  
- High False Alarm Rates (FAR) reduce the reliability of IDS solutions.  
- Difficulty in accurately detecting minority attacks such as U2R (User-to-Root) and R2L (Remote-to-Local).  
- Deep learning IDS approaches are accurate but computationally expensive for real-time systems.  

---

## Improvements Made in This Work
- Implemented and tested **Decision Tree variations** such as CART, ID3, and C4.5.  
- Applied **data preprocessing techniques** including feature scaling, normalization, and encoding of categorical variables.  
- Used **SMOTE-based balancing** to handle class imbalance and improve detection of minority attack types.  
- Performed **hyperparameter tuning** using GridSearchCV to optimize model depth and split criteria.  
- Evaluated performance using **Accuracy, Detection Rate (DR), and False Alarm Rate (FAR)** metrics.  

---

## Methodology
1. **Dataset Used:** NSL-KDD dataset for training and testing IDS models.  
2. **Preprocessing:** Encoded categorical features (`protocol_type`, `service`, `flag`), normalized numeric data, and removed unnecessary columns.  
3. **Model Development:**  
   - Baseline Decision Tree (imbalanced dataset)  
   - Class-Weighted Decision Tree (balanced by class weights)  
   - SMOTE Decision Tree (balanced using synthetic data)  
4. **Evaluation Metrics:** Accuracy, Detection Rate (DR), False Alarm Rate (FAR), Precision, Recall, and F1-Score.  

---

## Results
| Metric | Baseline DT | Weighted DT | SMOTE DT |
|--------|--------------|-------------|-----------|
| **Accuracy** | 76.0% | 76.0% | **92.7%** |
| **Detection Rate (DR)** | 83.4% | 86.0% | **90.3%** |
| **False Alarm Rate (FAR)** | 9.2% | 8.1% | **4.8%** |

- The optimized Decision Tree model achieved **92.7% accuracy** and a **90.3% detection rate** while reducing false alarms to **4.8%**.  
- Balancing the dataset using SMOTE significantly improved detection of minority attacks (R2L, U2R).  
- The model remained computationally efficient and interpretable, making it suitable for real-time IDS.  

---

## Conclusion
- The optimized Decision Tree–based Intrusion Detection System outperformed the baseline models in both accuracy and reliability.  
- Improvements in **feature preprocessing, data balancing, and parameter tuning** reduced false alarms and improved detection of rare attacks.  
- This work demonstrates that lightweight machine learning models like Decision Trees can achieve strong performance for IDS when properly optimized.  

---

## Technologies Used
- Python 3.12  
- pandas, scikit-learn, imbalanced-learn, matplotlib  
- Jupyter Notebook / VS Code  
- Dataset: NSL-KDD  

---

## References
1. *Comparative Analysis of Intrusion Detection Systems and Machine Learning-Based Model Analysis Through Decision Tree*, IEEE Xplore, 2023.  
   [https://ieeexplore.ieee.org/document/10185955](https://ieeexplore.ieee.org/document/10185955)  
2. NSL-KDD Dataset – [https://www.unb.ca/cic/datasets/nsl.html](https://www.unb.ca/cic/datasets/nsl.html)  
3. Scikit-learn Documentation – [https://scikit-learn.org](https://scikit-learn.org)
