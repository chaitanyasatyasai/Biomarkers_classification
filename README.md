# Biomarker Classification Project
Spark Tank-2k23
# Project Description:

This project focuses on classifying cancer biomarkers using various machine learning algorithms, including Support Vector Machine (SVM), Decision Tree, Random Forest, K-Nearest Neighbors (KNN), Logistic Regression, and Naive Bayes. The goal is to accurately predict the type of biomarker based on a set of molecular properties such as molecular weight, stability, specificity, and various cancer marker levels.

# Special Thanks
A special thanks to Dr.Vishnu Vardhan (M.D),Hyderabad for his invaluable guidance and expertise in the field of cancer biomarkers, which greatly contributed to the development of this project.


Note: This project is still a work in progress, and more features and optimizations are planned.

# Table of Contents
Installation
Usage
Contribution
Data Analysis
Models Used
Current Status
Future Work


# Installation
Clone the repository:
git clone https://github.com/chaitanyasatyasai/biomarker-classification.git
cd biomarker-classification
Install the required dependencies:

pip install -r requirements.txt
Add the dataset file biomarker_classification_final.xlsx to the /content/drive/MyDrive/ directory.

# Usage
Run the main Python script to train and test the models:

python sparktank.py
The script will load the dataset, handle missing values, and split the data into training and testing sets. It will then fit multiple models and output the accuracy of each model

# Contributing:
This project is being developed by a team of five members.
I am the team leader, responsible for Model training, including data pre-processing,data collection and for finding conclusions.


### Data Analysis

The dataset seems to consist of biomarker levels for 5000 patients, which may help in the classification or diagnosis of specific conditions, possibly cancer, given the presence of common cancer markers like CA 125, CA 19-9, CEA, etc.

Here’s a breakdown of the key statistics:

#### 1. **Molecular Weight** (MW):
- **Mean:** 38.65 
- **Std Dev:** 18.42
- **Range:** 13.70 to 76.80
- The molecular weight data is moderately spread, suggesting variability among samples.

#### 2. **Stability**:
- **Mean:** 1.20
- **Std Dev:** 0.78
- **Range:** 0 to 2
- This shows that most of the samples have high stability values, with the distribution leaning toward 1-2.

#### 3. **Sensitivity & Specificity**:
- **Mean:** 1.55 
- **Std Dev:** 2.87
- **Range:** 0.79 to 21.9
- The high standard deviation and range suggest large variations in sensitivity and specificity, possibly reflecting a mix of diagnostic performance across patients.

#### 4. **CA-125 Level (ng/mL)**:
- **Mean:** 2.26 
- **Std Dev:** 4.30
- **Range:** 0.1 to 21.86
- CA-125 levels are critical for detecting ovarian cancer. While the mean is low, the wide range and standard deviation indicate outliers or patients with potentially elevated cancer markers.

#### 5. **HE4 Level (ng/mL)**:
- **Mean:** 11.92
- **Std Dev:** 16.98
- **Range:** 0.1 to 69.2
- HE4 is another ovarian cancer marker, and its wide range suggests significant variability in the patient sample.

#### 6. **EGFR Level (ng/mL)**:
- **Mean:** 17.38 
- **Std Dev:** 20.05
- **Range:** 0.1 to 79.9
- This reflects the levels of the epidermal growth factor receptor, which can indicate different cancer types, particularly lung cancer. The data has a wide range and is highly variable.

#### 7. **ALK Level (ng/mL)**:
- **Mean:** 16.02 
- **Std Dev:** 16.80
- **Range:** 0.1 to 78.67
- ALK mutations are often found in lung cancer. The data shows a wide distribution of ALK levels.

#### 8. **ER Level (ng/mL)**:
- **Mean:** 11.79 
- **Std Dev:** 16.23
- **Range:** 0.1 to 78.23
- ER is relevant for estrogen receptors, often involved in breast cancer. The wide spread suggests significant differences among patients.

#### 9. **HERP Level (ng/mL)**:
- **Mean:** 16.70 
- **Std Dev:** 11.52
- **Range:** 0.1 to 74.50
- HERP shows a lower spread compared to other markers, but still has some outliers.

#### 10. **CA 19-9 Level (ng/mL)**:
- **Mean:** 17.34
- **Std Dev:** 17.44
- **Range:** 0.1 to 74.30
- A marker for gastrointestinal cancers. There’s a wide distribution with many outliers or extreme cases.

#### 11. **KRAS Level (ng/mL)**:
- **Mean:** 14.91
- **Std Dev:** 15.25
- **Range:** 0.1 to 74.5
- KRAS mutations are relevant to various cancers. Again, the data shows a wide range and standard deviation.

#### 12. **CEA Level (ng/mL)**:
- **Mean:** 17.57
- **Std Dev:** 15.58
- **Range:** 0.1 to 74.2
- CEA is used for colorectal and other types of cancers. The wide variability in the data suggests that not all patients have elevated levels.

#### 13. **BRAF Level (ng/mL)**:
- **Mean:** 17.62
- **Std Dev:** 16.51
- **Range:** 0.1 to 74.5
- BRAF mutations are often found in melanoma and other cancers. Similar to the other markers, there’s significant variation.

---

### Insights:
- Many biomarkers show a wide range of values with high standard deviations, indicating that some patients may have elevated levels, potentially correlating with cancer presence.
- Most of the biomarkers have medians lower than their means, suggesting the data might be skewed by outliers with exceptionally high values.
- The cancer markers such as CA-125, HE4, and CEA exhibit notable variation, which could imply differences in cancer stages or types across the patient population.

Further analysis, such as clustering or classification, might be useful in identifying subgroups or patterns in the data related to cancer diagnosis or progression.

# Models Used
The following machine learning models have been implemented in this project:

Support Vector Machine (SVM)

Decision Tree

Random Forest

K-Nearest Neighbors (KNN)

Logistic Regression

Naive Bayes

# Current Status
Data pre-processing is complete.
Initial implementation of multiple classification algorithms has been done.
Performance metrics such as accuracy are being calculated for each model.
The project is still in development, with future improvements planned.

# Future Work
Implement hyperparameter tuning for improved accuracy.
Add more advanced machine learning models.
Explore deep learning approaches to classification.
Optimize the model training and testing process.
Improve the handling of missing or inconsistent data.


# References
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6436208/pdf/13048_2019_Article_503.pdf
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9569881/pdf/ijms-23-12041.pdf
# Sites
https://biomarkerres.biomedcentral.com/
