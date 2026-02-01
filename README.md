# Diabetes Prediction Project

This project predicts diabetes risk using a Deep Learning model on a health dataset with 700k rows.

## Project Overview

1. **EDA & Visualization**
   - Checked for missing data (none found)
   - Explored distributions of numerical and categorical variables
   - Correlation analysis

2. **Feature Engineering**
   - Categorical variables converted with one-hot encoding
   - New features: `cholesterol_ratio`, `activity_screen_ratio`
   - StandardScaler applied for feature scaling

3. **Model Training**
   - Dense Neural Network with 4 hidden layers
   - ReLU activation in hidden layers, Sigmoid in output
   - Binary crossentropy loss, AUC metric
   - EarlyStopping to prevent overfitting
   - Validation AUC: 0.6953

4. **Predictions & Submission**
   - Generated predictions on the test set
   - Created Kaggle-ready `submission.csv`

5. **Visualization**
   - Loss and AUC plots for training and validation

6. **Streamlit Deployment**
   - Streamlit app prepared for Hugging Face Spaces
   - Users can input data and get diabetes probability
