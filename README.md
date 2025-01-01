# Building Machine Learning Pipelines for Predicting Pediatric Bone Marrow Transplant Survival

## Project Overview

This project leverages a dataset containing bone marrow transplantation characteristics for pediatric patients from the UCI Machine Learning Repository. The primary objective is to build a comprehensive machine learning pipeline that encompasses all preprocessing and data cleaning steps, ultimately selecting the best classifier to predict patient survival status.

## Dataset Description

The dataset includes various features related to both donors and recipients of hematopoietic stem cells. Key features of interest include:

- **donor_age**: The age of the donor at the time of hematopoietic stem cell apheresis.
- **donor_age_below_35**: Indicator of whether the donor's age is below 35 (yes, no).
- **donor_ABO**: ABO blood group of the donor (0, A, B, AB).
- **donor_CMV**: Presence of cytomegalovirus infection in the donor before transplantation (present, absent).
- **recipient_age**: Age of the recipient at the time of transplantation.
- **recipient_age_below_10**: Indicator of whether the recipient's age is below 10 (yes, no).
- **recipient_age_int**: Discretized intervals of the recipient's age (0,5], (5, 10], (10, 20].
- **recipient_gender**: Gender of the recipient (female, male).
- **recipient_body_mass**: Body mass of the recipient at the time of transplantation.
- **survival_status**: Survival status (0 - alive, 1 - dead).

## Project Steps

1. **Data Loading**:
   - Load the dataset into a DataFrame named `df`.

2. **Data Preprocessing**:
   - Identify and separate numerical and categorical columns.
   - Process numerical and categorical data appropriately, considering that all imported data are numeric. Binary columns (e.g., `donor_age_below_35`) are encoded as 0 and 1, and categorical columns (e.g., `donor_ABO`) are encoded as -1, 0, 1, and 2.

3. **Pipeline Construction**:
   - Construct a machine learning pipeline that handles data preprocessing, including scaling and encoding.
   - Ensure the pipeline processes numerical and categorical columns separately.

4. **Model Selection**:
   - Implement various classifiers and select the best-performing model based on evaluation metrics.
   - Use cross-validation to ensure the robustness of the selected model.

5. **Evaluation and Analysis**:
   - Evaluate the performance of the chosen model using metrics such as accuracy, precision, recall, and F1-score.
   - Analyze the results to draw insights and conclusions about the factors influencing pediatric bone marrow transplant survival.

## Conclusion

This project demonstrates the construction of a machine-learning pipeline to predict the survival status of pediatric bone marrow transplant patients. By preprocessing the data and selecting the best classifier, we aim to enhance the predictive accuracy and provide valuable insights into the factors affecting patient outcomes.
### Output
![image](https://github.com/user-attachments/assets/7da550bc-1220-4580-9395-1a4ee451adb3)


## Dataset Source

The dataset used in this project is available at the UCI Machine Learning Repository: [Bone Marrow Transplantation Dataset](https://archive.ics.uci.edu/ml/datasets/Bone+Marrow+Transplantation).

## Repository Structure

- **data/**: Contains the dataset used for the project.
- **notebooks/**: Jupyter notebooks with exploratory data analysis, pipeline construction, and model training.
- **scripts/**: Python scripts for data preprocessing, model training, and evaluation.
- **results/**: Evaluation metrics and analysis results.
- **README.md**: Project overview and detailed explanation of the steps involved.

## Getting Started

To reproduce the results, follow these steps:

1. Clone the repository.
2. Install the necessary dependencies.
3. Run the preprocessing script to prepare the data.
4. Execute the model training script to build and evaluate the pipeline.

Feel free to explore the notebooks and scripts to understand the detailed implementation of the project.

---

By building a robust machine learning pipeline, this project aims to contribute to the predictive modeling of pediatric bone marrow transplantation outcomes, potentially aiding in better decision-making and improved patient care.
