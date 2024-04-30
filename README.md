# Heart Disease Prediction Using Random Forest

This repository contains a project focused on predicting heart disease using a Random Forest classifier. The dataset used for training and testing the model is available in `heart.csv`. The dataset contains information about various attributes that can influence a person's likelihood of having heart disease.

## Dataset Description
Dataset is publicly available : https://www.kaggle.com/datasets/arezaei81/heartcsv

The dataset consists of 304 rows, each representing a patient, with the following attributes:

- `age`: The person's age in years
- `sex`: The person's sex (1 = male, 0 = female)
- `cp`: The type of chest pain experienced (1: typical angina, 2: atypical angina, 3: non-anginal pain, 4: asymptomatic)
- `trestbps`: The person's resting blood pressure (mm Hg on admission to the hospital)
- `chol`: The person's cholesterol measurement in mg/dl
- `fbs`: The person's fasting blood sugar (> 120 mg/dl, 1 = true; 0 = false)
- `restecg`: Resting electrocardiographic measurement (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy by Estes' criteria)
- `thalach`: The person's maximum heart rate achieved
- `exang`: Exercise-induced angina (1 = yes; 0 = no)
- `oldpeak`: ST depression induced by exercise relative to rest
- `slope`: The slope of the peak exercise ST segment (1: upsloping, 2: flat, 3: downsloping)
- `ca`: The number of major vessels (0-3)
- `thal`: A blood disorder called thalassemia (3 = normal, 6 = fixed defect, 7 = reversible defect)
- `target`: Heart disease (0 = no, 1 = yes)

## Analysis and Model Training

The analysis begins with exploring the dataset's correlation matrix to understand how each parameter affects a person's heart condition. After splitting the data into training and testing sets, a Random Forest classifier with a maximum depth of 5 is trained on the training data. The trained model is then used to predict heart disease on the testing data.

## Results

The model's performance is evaluated using a confusion matrix, which shows the model's ability to correctly identify instances of heart disease. Additionally, the receiver operating characteristic (ROC) curve is plotted to visualize the trade-off between true positive rate (sensitivity) and false positive rate (1 - specificity). The area under the ROC curve (AUC) is calculated to assess the model's overall performance. For this model, the AUC is approximately 0.909, and the accuracy is approximately 82.42%.

## Usage

To run the project:

1. Clone the repository.
2. Install the required dependencies (such as pandas, numpy, matplotlib, seaborn, scikit-learn).
3. Run the provided Python script to train the model and evaluate its performance.

```bash
Heart Disease Classification.ipynb
