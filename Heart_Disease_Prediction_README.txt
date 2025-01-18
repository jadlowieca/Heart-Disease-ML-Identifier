
# Heart Disease Prediction Notebook

This Jupyter notebook provides a machine learning model to predict the likelihood of heart disease based on user inputs. The model uses the RandomForestClassifier and one-hot encoding for categorical data.

## Requirements

Before running the notebook, you must install the following dependencies:

1. Python 3. (preferably Python 3.7+)
2. Jupyter Notebook - To run the notebook environment.

### Python Libraries:
- pandas
- ipywidgets
- scikit-learn
- matplotlib


### Machine Learning Pipeline
1. Data Preprocessing: 
    - Categorical features (`Sex`, `ChestPainType`, `RestingECG`, `ExerciseAngina`, `ST_Slope`) are one-hot encoded using `ColumnTransformer`.
    - Numeric features are left unchanged.
2. Model:
    - A Random Forest Classifier is used to predict the probability of heart disease.
    - The classifier is trained on the heart disease dataset, split into training and testing sets.

### Training and Evaluation
The model is trained using the following data split:
- 80% for training
- 20% for testing

The model’s accuracy is evaluated on the test set using the `.score()` method.

1. Model Training: 
    - The model is trained with RandomForestClassifier using the `fit()` method.
    - Predictions are made with `predict()` and `predict_proba()` to return the prediction and probability.
    
2. User Input: 
    - The widgets capture user input values and pass them into the trained model.
    - The probability of heart disease is then displayed to the user.
