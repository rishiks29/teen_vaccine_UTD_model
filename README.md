# rishik_research_repository
Author: Rishik Shenolikar
Description: Machine learning framework using CDC NIS-Teen data to predict adolescent vaccination status and generate socioecological risk tiers for targeted public health outreach.

## Overview
Vaccination is a cornerstone of public health, yet disparities in adolescent vaccination uptake persist across demographic and socioeconomic groups. This project develops a machine learning framework to predict vaccination status using nationally representative survey data and to identify high-risk populations for targeted outreach.

Using data from the National Immunization Survey-Teen (NIS-Teen), multiple classification models were evaluated to assess predictive performance and interpret key drivers of vaccination behavior.

---

## Research Objective
The goal of this project is to:

- Predict adolescent vaccination status using demographic, healthcare access, and socioeconomic variables  
- Compare the performance of multiple machine learning models  
- Identify key predictors influencing vaccination uptake  
- Develop risk-tier classifications to support targeted public health interventions  

---

## Dataset
**Source:** National Immunization Survey-Teen (NIS-Teen)  
**Type:** Public health survey data  

The dataset includes:
- Demographics (age, region, race/ethnicity)
- Healthcare access variables
- Preventive care indicators
- Provider recommendation variables  

**Note:**  
Due to data use restrictions, the raw dataset is not included in this repository. The code provided reproduces the full preprocessing and modeling pipeline.

---

## Methodology

### 1. Data Preprocessing
- Handling missing values  
- Encoding categorical variables  
- Feature selection based on literature and domain relevance  
- Train-test split for model evaluation  

### 2. Model Development
Models evaluated include:
- Logistic Regression (L1 regularization / LASSO)  
- Random Forest  
- Gradient Boosting  
- Additional baseline classifiers  

### 3. Model Evaluation
Performance metrics:
- AUROC  
- F1 Score  
- Accuracy  
- Balanced Accuracy  
- Precision & Recall  

### 4. Risk Stratification
Predicted probabilities were used to classify individuals into:
- Low-risk  
- Medium-risk  
- High-risk  

These tiers can inform targeted vaccination outreach strategies.

---

## Key Findings
- Regularized logistic regression demonstrated strong and stable performance across evaluation metrics  
- More complex models provided limited improvement, suggesting largely linear relationships in the dataset  
- Provider recommendation and healthcare access variables were among the strongest predictors  
- Risk-tiering enables practical application for population-level intervention strategies
 
---

## Reproducibility
This repository contains all code necessary to:
- preprocess the dataset  
- train machine learning models  
- evaluate performance metrics  

Because the NIS-Teen dataset is restricted, users must obtain access separately. Once obtained, the provided pipeline can be used to reproduce results.

---

## Limitations
- The dataset consists primarily of structured survey variables, which may limit the ability of complex models to outperform simpler approaches  
- Survey weighting was not applied in model training, which may affect generalizability to the full U.S. population  
- Some predictor variables may not be readily available in real-time clinical settings  

---

## Future Work
- Incorporate survey weights into modeling  
- Explore additional feature engineering techniques  
- Evaluate model performance on other vaccination datasets  
- Develop deployment tools for real-time risk prediction  

---

## Acknowledgments
This project was conducted as part of independent student research in public health and machine learning.

---

## License
This project is intended for educational and research purposes.
