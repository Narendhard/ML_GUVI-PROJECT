# BREAST CANCER PREDICTION MODEL

***OVERVIEW***
# OVERVIEW

This project implements a machine learning model to predict whether a breast tumor is benign or malignant based on various diagnostic features. The model is trained using the Breast Cancer Wisconsin Dataset and evaluated for its performance. The Random Forest Classifier is utilized for classification, and the results include a classification report, confusion matrix, and feature importance visualization.

***DATASET***
# DATASET

The dataset used in this project is BreastCancer.csv. It contains diagnostic measurements of breast tumors. The key columns in the dataset are:

@@ -22,7 +22,7 @@ radius_se, texture_se, perimeter_se, etc.

radius_worst, texture_worst, perimeter_worst, etc.

***PREREQUISITES***
# PREREQUISITES

To run the code, you need the following libraries installed:

@@ -42,7 +42,7 @@ Install them using:

pip install pandas numpy scikit-learn matplotlib seaborn

***STEPS IN THE CODE***
# STEPS IN THE CODE

Import Libraries: Necessary libraries are imported for data processing, model training, evaluation, visualization, and serialization.

@@ -72,7 +72,7 @@ The importance of each feature in prediction is visualized using a bar plot.
**Model Serialization:**
The trained model is saved as a pickle file (breast_cancer_model.pkl) for later use.

***HOW TO RUN***
# HOW TO RUN

Save the dataset as BreastCancer.csv in the working directory.

@@ -90,7 +90,7 @@ Feature importance visualization.

Serialized model file (breast_cancer_model.pkl).

***EXPECTED OUTPUTS***
# EXPECTED OUTPUTS

**Correlation Heatmap:** Displays relationships between features.

@@ -100,16 +100,18 @@ Serialized model file (breast_cancer_model.pkl).

**Feature Importance Plot:** Highlights which features are most important for the predictions.

***USAGE OF PICKLE FILE***
# USAGE OF PICKLE FILE

The trained model is saved as a pickle file for reuse:
import pickle

**Load the saved model**
with open('breast_cancer_model.pkl', 'rb') as f:
    model = pickle.load(f)

**Use the model for prediction**
prediction = model.predict(new_data)
print("Prediction:", prediction)
