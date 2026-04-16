# Blood-Donation-Prediction
# Blood Donation Prediction (Predicting Future Donors)

This project utilizes historical blood donation data to predict whether a donor will return to donate in a target period. By identifying donation patterns, healthcare organizations can better manage blood supply and target recruitment efforts.

## Key Results
* **Primary Model:** K-Nearest Neighbors (KNN)
* **Performance:** Achieved a cross-validated accuracy of **79.34%**.
* **Key Insight:** Recency (months since last donation) and Frequency (total donations) are critical indicators of future donor behavior.

## Dataset Features
The dataset tracks donor history with the following metrics:
- **Months since Last Donation:** Recency of the donor's last visit.
- **Number of Donations:** Frequency of donations.
- **Total Volume Donated (c.c.):** Total amount of blood contributed.
- **Months since First Donation:** Time since the donor's first recorded donation.
- **Made Donation in March 2007:** The target variable (1 = Yes, 0 = No).

## Tech Stack
- **Language:** Python
- **Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn (Logistic Regression, KNN, Random Forest, SVM)

## Project Workflow
1. **Exploratory Data Analysis (EDA):** Investigated donation frequency and the impact of time since first/last donation.
2. **Preprocessing:** - Feature scaling using `StandardScaler` (essential for distance-based models like KNN).
   - Analysis of class distribution to understand donor patterns.
3. **Model Selection:** Compared multiple classification algorithms:
   - K-Nearest Neighbors (KNN)
   - Random Forest Classifier
   - Logistic Regression
   - Support Vector Machine (SVM)
4. **Hyperparameter Tuning:** Optimized KNN using `GridSearchCV` to find the ideal number of neighbors and weight functions.
5. **Evaluation:** Detailed analysis using accuracy scores and classification reports.

## Conclusion
The study demonstrated that KNN is an effective model for this classification task. While tuning improved cross-validation performance, the project highlights the importance of feature engineering in handling limited numeric datasets.
