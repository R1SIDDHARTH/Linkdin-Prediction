# Project: LinkedIn Data Analysis and Skill Prediction

This project is aimed at analyzing LinkedIn data, specifically for job postings and applicant skills, and predicting skill requirements using machine learning models. The project uses logistic regression and random forest classifiers to predict the likelihood of a candidate possessing specific skills, such as Python or Java, based on provided features.

## Features

- **Data Extraction**: Unzipping and loading the dataset from a provided zip file.
- **Data Preprocessing**: Filtering data based on companies, such as Infosys, and preparing it for model training.
- **Skill Prediction**: Logistic Regression and Random Forest models are used to predict the likelihood of a candidate possessing a certain skill.
- **Model Evaluation**: Evaluation is done using classification reports and confusion matrices.
- **Feature Importance**: Visualizing feature importance for predicting skills.

## Prerequisites

To run this project, you need the following Python libraries installed:

- `pandas`: For data manipulation.
- `numpy`: For numerical operations.
- `scikit-learn`: For machine learning models.
- `matplotlib` and `seaborn`: For data visualization.
- `zipfile` and `os`: For file handling and extraction.

You can install the required libraries using pip:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Workflow

1. **Unzipping the Dataset**:
   - The project starts by unzipping the LinkedIn data from a zip file and extracting the contents to a specified folder.

2. **Data Loading**:
   - The extracted CSV file is loaded into a pandas DataFrame for further analysis.

3. **Skill Prediction Using Logistic Regression**:
   - Predicts whether a candidate has Python skills based on features extracted from the dataset.
   - Evaluation is performed using a classification report and confusion matrix.
   - Visualizes feature importance for Python skill prediction.

4. **Company-Specific Analysis**:
   - Filters data for job postings specific to companies like Infosys.
   - Analyzes the distribution of total applicants for Infosys.

5. **Skill Prediction Using Random Forest**:
   - A Random Forest model is used to predict Java skills.
   - Similar evaluation steps are carried out, including feature importance visualization.

## Visualizations

- **Confusion Matrix**: A heatmap showing the performance of the model in terms of correctly and incorrectly predicted categories.
- **Feature Importance**: Bar plots showing the most significant features used by the model to predict skills.
- **Correlation Matrix**: Heatmaps displaying the correlations between different skills.

## How to Run

1. Clone the repository and unzip the dataset.
2. Make sure all the dependencies are installed.
3. Run the Python script to execute the workflow.

```bash
python linkedin_skill_prediction.py
```

## Results

- **Skill Prediction Accuracy**: The logistic regression and random forest models provide an accuracy score along with detailed metrics like precision, recall, and F1-score.
- **Feature Importance**: The features used in the models are ranked based on their importance in predicting skills like Python or Java
