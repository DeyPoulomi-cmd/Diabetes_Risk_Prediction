# Diabetes Risk Prediction

This repository contains a comprehensive analysis and implementation of a predictive model for identifying diabetes risk using machine learning techniques. The project leverages data preprocessing, feature engineering, and multiple classification algorithms to deliver high-accuracy predictions.

---

## Overview

Diabetes is a global health concern, and early identification of at-risk individuals can help in timely interventions. This project aims to develop a predictive model to classify individuals as diabetic or non-diabetic based on their physiological attributes.

---

## Features of the Project

1. **Data Analysis**:
   - Explored and visualized key trends in the dataset, including the distribution of features like glucose levels, BMI, and insulin.
   - Conducted correlation analysis to identify significant predictors of diabetes.

2. **Preprocessing Pipeline**:
   - Handled missing values and outliers effectively.
   - Scaled numerical features for model optimization.
   - Engineered new features to enhance model performance.

3. **Modeling**:
   - Implemented various machine learning algorithms, including Logistic Regression, Decision Trees, and Random Forests.
   - Random Forest achieved the highest accuracy of **88%**.

4. **Evaluation**:
   - Used accuracy, precision, recall, and ROC-AUC to evaluate model performance.

---

## Insights and Learnings

1. **What did I learn?**
   - Developed a strong understanding of how glucose levels, BMI, and age serve as critical predictors of diabetes.
   - Learned effective techniques to preprocess and balance datasets for improved machine learning outcomes.
   - Gained insights into model performance metrics and their role in evaluating classification models.

2. **What did I try out?**
   - Explored multiple machine learning algorithms, including Logistic Regression, Decision Trees, and Random Forests, to identify the best-performing model.
   - Experimented with hyperparameter tuning to optimize Random Forest performance.
   - Used SMOTE (Synthetic Minority Oversampling Technique) to handle class imbalance effectively.

3. **What worked and why?**
   - Random Forest outperformed other models, achieving an accuracy of 88%, due to its ability to handle feature interactions and non-linear relationships.
   - Preprocessing steps such as scaling and outlier handling ensured a robust dataset for model training.
   - SMOTE improved model recall, making it more effective in identifying diabetic cases.

4. **Recommendations for the Business Counterpart**
   - Regularly monitor glucose levels and BMI as part of routine health checkups to identify high-risk individuals early.
   - Implement targeted interventions for high-risk groups to prevent the onset of diabetes.
   - Update the dataset periodically and retrain the model to maintain its accuracy and relevance.

---

## Dataset

The dataset used in this project is sourced from the National Institute of Diabetes and Digestive and Kidney Diseases. It contains the following key features:

- **Pregnancies**: Number of pregnancies.
- **Glucose**: Plasma glucose concentration.
- **BloodPressure**: Diastolic blood pressure.
- **SkinThickness**: Triceps skinfold thickness.
- **Insulin**: 2-hour serum insulin.
- **BMI**: Body mass index.
- **DiabetesPedigreeFunction**: Family history of diabetes.
- **Age**: Age of the individual.
- **Outcome**: Target variable (0 = Non-Diabetic, 1 = Diabetic).

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/diabetes-risk-prediction.git
   ```

2. Navigate to the project directory:
   ```bash
   cd diabetes-risk-prediction
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. Run the Jupyter Notebook to explore the data and train models:
   ```bash
   jupyter notebook Diabetes_Risk_Prediction.ipynb
   ```

2. To evaluate the trained model:
   ```python
   from sklearn.metrics import accuracy_score

   y_pred = model.predict(X_test)
   accuracy = accuracy_score(y_test, y_pred)
   print(f"Model Accuracy: {accuracy:.2f}")
   ```

---

## Results

- **Accuracy**: 88%
- **Key Predictors**: Glucose, BMI, and Age
- **Impact**: Improved prediction reliability by 20%, aiding early identification of at-risk individuals.

---

## Recommendations

Based on the analysis and findings:

1. Focus on monitoring glucose levels and BMI for early detection.
2. Provide personalized health interventions for high-risk individuals.
3. Regularly update the dataset and retrain the model to maintain accuracy.

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-branch
   ```
5. Open a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgments

- National Institute of Diabetes and Digestive and Kidney Diseases for providing the dataset.
- Open-source contributors and the machine learning community for their valuable resources.

---

Thank you for exploring this project! If you have any questions or suggestions, feel free to reach out.
