# Graduate Employability Analysis

This project explores a graduate employability dataset to identify which student characteristics have the strongest impact on job placement outcomes.  
The focus is to understand what truly matters for employability: GPA? Communication skills? IQ? Project experience? Or something else?

The analysis uses a Random Forest classifier and permutation-based feature importance to evaluate which attributes contribute most to predicting whether a student gets placed.

---

## Dataset Overview

Each row represents one student, with fields including:

- IQ  
- Previous Semester Result  
- CGPA (converted to a 4.0 scale)  
- Academic Performance  
- Internship Experience (Yes/No)  
- Extra-Curricular Score  
- Communication Skills  
- Projects Completed  
- Placement outcome (Yes/No)

### GPA Conversion  
The dataset originally used a 10-point CGPA scale. I standardized it using:

GPA_4 = (CGPA/10) * 4

This allows the results to be interpreted on a conventional 4.0 scale.

---

## Objective

**Which features are the strongest predictors of whether a student gets placed?**

To answer this, the project applies:

- Random Forest classification  
- Permutation feature importance  
- Accuracy evaluation  
- Visual analysis (bar plot of feature importance)

---

## Key Results

### **Top Predictors of Student Placement**
Based on permutation importance:

1. **Communication Skills** – most influential predictor  
2. **GPA (4.0 scale)** – strong academic signal  
3. **IQ** – meaningful cognitive indicator  
4. **Projects Completed** – moderate contribution  

### **Minimal or No Impact**
These features had little or no effect on prediction:

- Previous Semester Result  
- Academic Performance Rating    
- Extra-Curricular Score  

### **Overall Insight**

Communication skills, GPA, IQ, and hands-on project experience were the dominant factors in this dataset.  
Traditional metrics such as academic rating, extracurriculars, flags contributed very little to prediction accuracy.

---

## Model Performance

Accuracy:  
