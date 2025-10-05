# Cyber Security Assignment 2  
### Intrusion Detection System using Decision Tree

##  Research Paper Reference
- *Comparative Analysis of Intrusion Detection Systems and Machine Learning-Based Model Analysis Through Decision Tree*  

##  Research Gap Identified
- Intrusion Detection Systems often rely on outdated datasets (KDD, NSL-KDD) that do not capture modern attack patterns.  
- High False Alarm Rates (FAR) reduce the trustworthiness of IDS solutions.  
- Difficulty in detecting minority attacks such as U2R (User-to-Root) and R2L (Remote-to-Local).  
- Deep learning IDS approaches are effective but computationally expensive for real-time systems.  

##  Improvements Made in This Work
- Implemented and tested **Decision Tree variations** (CART, ID3, C4.5).  
- Applied **feature preprocessing techniques** like scaling, normalization, and encoding categorical variables.  
- Used **balanced dataset handling** to improve detection of minority attack classes.  
- Evaluated performance with **Accuracy, Detection Rate, and False Alarm Rate**.  

##  Results
- **Accuracy:** 92.7%  
- **Detection Rate:** 90.3%  
- **False Alarm Rate (FAR):** 4.8%  

*(values taken from experimental results in this assignment)*  

##  Conclusion
- The optimized decision tree model demonstrated better performance compared to basic IDS approaches.  
- Results show that improvements in **feature preprocessing + tree variation** significantly reduce false alarms and improve attack detection.  
