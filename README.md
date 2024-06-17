The goal is to predict the likelihood of individuals receiving the xyz and seasonal flu vaccines. The dataset contains 36 columns, including respondent_id and 35 features. Initially, columns with a large number of missing values were dropped. Missing values in the remaining columns were filled using the mode with SimpleImputer. Categorical variables were label encoded. Logistic Regression models were trained separately for predicting both the variables(xyz_vaccine and seasonal_vaccine) , and the model performance was evaluated using the ROC AUC score, which measures the model's ability to distinguish between the classes.
