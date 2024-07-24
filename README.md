# Predicting Term Deposit Subscription by a Client

## Overview
This project aims to predict whether a client will subscribe to a term deposit when contacted by a marketing agent. By analyzing various client attributes and previous campaign data, we use Support Vector Machine (SVM) for the predictive analytics.

## Data Details
The dataset contains information related to direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls, and multiple contacts were often made to the same client.

### Variable Description:
- **age**: Age of the client
- **job**: Type of job (categorical)
- **marital**: Marital status (categorical)
- **education**: Education level (categorical)
- **default**: Credit in default? (categorical)
- **housing**: Has a housing loan? (categorical)
- **loan**: Has a personal loan? (categorical)
- **contact**: Contact communication type (categorical)
- **month**: Last contact month of the year (categorical)
- **day_of_week**: Last contact day of the week (categorical)
- **duration**: Last contact duration, in seconds
- **campaign**: Number of contacts performed during this campaign and for this client
- **pdays**: Number of days since the client was last contacted from a previous campaign
- **previous**: Number of contacts performed before this campaign for this client
- **poutcome**: Outcome of the previous marketing campaign (categorical)
- **emp.var.rate**: Employment variation rate - quarterly indicator
- **cons.price.idx**: Consumer price index - monthly indicator
- **cons.conf.idx**: Consumer confidence index - monthly indicator
- **euribor3m**: Euribor 3 month rate - daily indicator
- **nr.employed**: Number of employees - quarterly indicator
- **y**: Has the client subscribed a term deposit? (binary: 'yes','no')

## Project Workflow
1. **Data Preprocessing & Exploratory Data Analysis (EDA)**
   - Handle missing values
   - Encode categorical variables
   - Analyze the distribution of variables
   - Split the data into training and testing sets

2. **Model Building with Support Vector Machine (SVM)**
   - Train the SVM classifier
   - Make predictions on the testing set
   - Evaluate the model using various metrics

3. **Hyperparameter Tuning**
   - Tune the hyperparameters of the SVM model to improve performance

4. **Evaluation & Visualization**
   - Assess model performance using metrics like precision, recall, F1-score, and AUC-ROC
   - Visualize confusion matrix and ROC curve

## Data Preprocessing
- Encode categorical variables using Label Encoding
- Handle missing values by imputing or dropping missing data
- Split the data into features (X) and target variable (y)
- Perform train-test split with 80% training data and 20% testing data

## Model Building
- **Support Vector Machine (SVM)**: A robust classifier used for prediction
- **Hyperparameter Tuning**: Use techniques like grid search or random search to find the best parameters for the SVM model

## Scripts
- `term_deposit_subscription.py`: Contains code for preprocessing, EDA, model training, hyperparameter tuning, and evaluation.

## Evaluation Metrics
- **Accuracy**: Measures the overall correctness of the model
- **Precision**: Measures the correctness of positive predictions
- **Recall (Sensitivity)**: Measures the ability to identify positive instances
- **Specificity**: Measures the ability to identify negative instances
- **F1-Score**: Harmonic mean of precision and recall
- **AUC-ROC**: Measures the area under the receiver operating characteristic curve

## Running the Project
Open and run the `term_deposit_subscription.ipynb` notebook.**
