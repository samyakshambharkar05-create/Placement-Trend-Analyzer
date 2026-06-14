# Placement Trend Analyzer: ML-Based Student Placement and Salary Prediction System

**Author(s):** Samyak Shambharkar

**Affiliation:** Suryodaya College Of Engineering and Technology

**Date:** June 2026

---

# Abstract

The Placement Trend Analyzer is a Machine Learning-based system designed to predict student placement outcomes and expected salary packages based on academic performance, technical skills, internships, projects, and other career-related factors. The objective of this project is to assist students in understanding their employability status and identifying areas for improvement before participating in campus recruitment processes.

The project utilizes a placement dataset containing student academic records, technical skill assessments, internship experience, project work, certifications, and placement information. Multiple machine learning algorithms were evaluated for both classification and regression tasks. Logistic Regression was selected for placement prediction, achieving an accuracy of 69.78% and an F1-score of 0.81. For salary prediction, XGBoost Regressor produced the best performance with an R² score of 0.784, MAE of 0.963, and RMSE of 1.206.

A user-friendly dashboard was developed using Streamlit, allowing users to input their profile information and instantly obtain placement probability and salary predictions. The project demonstrates how machine learning can be applied to educational analytics and career planning to provide data-driven insights for students and institutions.

---

# Introduction

Campus placements play a significant role in determining the career opportunities available to students after graduation. Educational institutions and students often seek methods to evaluate employability and estimate expected salary packages based on academic and professional achievements.

Traditional placement preparation relies heavily on subjective assessment and historical observations. However, with the availability of educational data and machine learning techniques, it is possible to identify patterns that influence placement success and salary outcomes.

The objective of this project is to develop a predictive system capable of estimating whether a student is likely to secure placement and predicting the expected salary package. Such a system can help students improve weak areas, guide placement preparation, and support institutions in understanding placement trends.

---

# Literature Review

Several studies have explored the application of machine learning in educational data mining and employability prediction.

Researchers have used classification algorithms such as Logistic Regression, Decision Trees, Random Forests, and Support Vector Machines to predict student placement outcomes. These models analyze academic performance, aptitude scores, communication skills, and extracurricular activities to identify factors influencing employability.

Recent studies have also incorporated ensemble learning techniques such as XGBoost and Gradient Boosting for salary prediction due to their ability to capture complex relationships between variables. Educational analytics platforms increasingly utilize machine learning models to provide personalized career guidance and employability assessments.

This project builds upon these approaches by combining placement prediction and salary estimation within a single interactive dashboard.

---

# Methodology

The project follows a supervised machine learning approach. Initially, the dataset was imported and examined for missing values, duplicates, and data inconsistencies. Since the dataset contained no missing values, preprocessing mainly involved encoding categorical variables and preparing the data for model training.

Exploratory Data Analysis (EDA) was conducted to understand feature distributions and identify relationships between student attributes and placement outcomes. The dataset was then divided into training and testing subsets.

For placement prediction, Logistic Regression, Random Forest, and XGBoost classifiers were evaluated. Logistic Regression achieved the best overall performance and was selected as the final classification model.

For salary prediction, Linear Regression, Random Forest Regressor, Gradient Boosting Regressor, and XGBoost Regressor were compared. XGBoost produced the highest R² score and was selected as the final regression model.

The trained models were exported using Pickle and integrated into a Streamlit dashboard for real-time predictions.

---

# Implementation

### Programming Language

* Python

### Libraries and Frameworks

* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* Plotly
* Streamlit
* Pickle

### Development Environment

* Google Colab
* GitHub
* Streamlit Cloud

### Machine Learning Models

#### Classification Models

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

#### Regression Models

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost Regressor

---

# Results and Discussion

## Placement Prediction Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 69.78%   |
| Random Forest       | 68.94%   |
| XGBoost             | 69.55%   |

### Final Classification Model

**Logistic Regression**

Additional Metrics:

* Precision: 0.715
* Recall: 0.929
* F1 Score: 0.808

---

## Salary Prediction Results

| Model                       | R² Score |
| --------------------------- | -------- |
| Linear Regression           | 0.773    |
| Random Forest Regressor     | 0.762    |
| Gradient Boosting Regressor | 0.780    |
| XGBoost Regressor           | 0.784    |

### Final Regression Model

**XGBoost Regressor**

Additional Metrics:

* MAE: 0.963
* RMSE: 1.206

The results indicate that student skills, internships, projects, certifications, and academic performance contribute significantly to placement success and salary outcomes.

### Dashboard Screenshots

**Figure 1:** Streamlit Dashboard Home Page


**Figure 2:** Placement Prediction Result


**Figure 3:** Salary Prediction Result


---

# Limitations

1. The dataset is synthetic and may not perfectly represent real-world placement scenarios.
2. Placement decisions are influenced by factors not included in the dataset, such as interview performance and company-specific requirements.
3. Branch labels were encoded numerically, reducing interpretability.
4. The model's accuracy is limited by the quality and diversity of available features.
5. Predictions should be considered indicative rather than definitive outcomes.

---

# Future Scope

1. Incorporate real placement data collected from universities and training institutions.
2. Add resume analysis and skill extraction using Natural Language Processing (NLP).
3. Include interview performance metrics and coding assessment scores.
4. Develop personalized recommendations for improving placement probability.
5. Integrate real-time analytics and student performance tracking.
6. Deploy the application as a scalable cloud-based platform accessible to educational institutions.

---

# Conclusion

This project successfully demonstrates the application of machine learning techniques in predicting student placement outcomes and salary packages. Logistic Regression provided the most effective classification performance, while XGBoost Regressor achieved the best salary prediction results.

The developed Streamlit dashboard offers an interactive platform for students to evaluate their employability and expected salary package based on their academic and professional profiles. The project highlights the potential of educational analytics in supporting career planning and placement preparation through data-driven decision-making.

---

# References

[1] Han, J., Kamber, M., & Pei, J., "Data Mining: Concepts and Techniques," Morgan Kaufmann, 2011.

[2] Pedregosa, F. et al., "Scikit-Learn: Machine Learning in Python," Journal of Machine Learning Research, 2011.

[3] Chen, T., & Guestrin, C., "XGBoost: A Scalable Tree Boosting System," KDD Conference, 2016.

[4] Streamlit Documentation: https://streamlit.io

[5] Scikit-Learn Documentation: https://scikit-learn.org

[6] XGBoost Documentation: https://xgboost.readthedocs.io

[7] Kaggle Placement Prediction Dataset (2026): https://www.kaggle.com
