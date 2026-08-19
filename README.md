# Explainable AI-Based Lung Cancer Detection Using E-nose Breath Data 
## Overview 
This repository contains the implementation of explainable machine learning framework for lung cancer classification using electronic-nose (E-nose) breath sensor data. 

## Objective 
The primary objective of this study is to develop, non-invasive, and interpretable machine learning framework for the detection of lung cancer using VOC-based breath sensor data integrated with demographic variables and explainable AI techniques.

## Dataset 
The study used a publicly available E-nose breath sensor dataset obtained from the Breath_analysis repository. 

The dataset contains 118 samples, including: 
- 65 lung cancer samples
- 53 healthy control samples
- Responses from six semiconductor gas sensors
- Measurements recorded at three sensor operating temperatures
- Demographic and clinical information 

The dataset includes sensor responses together with variables such as age, sex, smoking status, lung cancer stage, and cancer type.

## Data Source 
The original dataset is available from: 
https://github.com/camberbatch/Breath_analysis 

## Methodology 
The overall framework consists of the following stages: 
1. Data preparation
2. Exploratory and statistical analysis
3. Machine learning classification
4. Model evaluation
5. Explainable AI analysis
6. Feature importance and ablation analysis

## Machine Learning 
Three machine learning classifier were used Logistic Regression, Random Forest, and XGBoost.
Model performance is evaluated using cross-validation and standard classification metrics.

## Explainable AI 
SHAP (SHapley Additive exPlanations) is used to investigate the contribution of individual features to model predictions. 
The analysis provides insight into the relative importance sensor and demographic variables used by the trained model.

## Feature Ablation 
A feature ablation analysis was conducted to further investigate the importance of features identified through model interpretation. 
Different feature subsets were evaluated to assess their contribution to classification performance. 

## Results 

Note : The reported results are based on the study dataset and validation framework and should not be interpreted as evidence of clinical diagnostic performance. 

## Repository structure 
├── README.md 

├── requirements.txt 

└── notebooks/

      ├── 01_Statistical_Analysis.ipynb
    
      ├── 02_LR & RF models.ipynb
    
      ├── 03_XGBoost_Model.ipynb
    
      ├── 04_Explainable_AI.ipynb
    
      └── 05_Ablation_analysis.ipynb

## Installation 
Clone the repository: 

git clone https://github.com/varshaghatage06/explainable-ai-breath-lung-cancer-detection.git

cd explainable-ai-breath-lung-cancer-detection 

Install the required Python packages in Colab notebook  : 

!pip install -r requirements.txt 

## Usage 
The Colab notebooks in the 'notebooks/' directory implement the main components of the analysis pipeline. 
The workflow includes data preprocessing, model development, performance evaluation, explainability analysis, and feature ablation.
Refer to the individual notebooks for execution details.

## Technologies 
- Python
- NumPy
- Pandas
- SciPy
- Scikit-learn
- XGBoost
- SHAP
- Imbalanced-learn
- Matplotlib

## Disclaimer 
This repository is intended for academic and research purposes only. 
The models and results presented here have not been established as a clinically validated diagnostic system and should not be used for medical diagnosis or clinical decision-making.
