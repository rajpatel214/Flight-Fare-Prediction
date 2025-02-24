# **Flight Fare Prediction Using Machine Learning**  

## **Project Overview**  
This project focuses on predicting flight ticket prices using machine learning techniques. The dataset includes various flight-related attributes, such as airline, source, destination, journey date, departure and arrival times, duration, total stops, and additional flight details. The main objective is to build a predictive model that accurately estimates ticket prices based on these features.  

## **Data Preprocessing**  
Before training the model, data preprocessing was performed to handle missing values, transform categorical features, and extract relevant information.  

1. **Handling Missing Values**:  
   - The dataset contained missing values in the "Total_Stops" column, which were imputed using the most frequent category based on the route.  

2. **Feature Engineering**:  
   - Journey date, departure time, and arrival time were extracted into separate numerical features (month, day, hour, minute).  
   - The "Duration" column was transformed into separate hour and minute features.  
   - Categorical variables such as airline, source, and destination were encoded using Label Encoding.  

3. **Feature Transformation**:  
   - The "Total_Stops" feature was converted from text format (e.g., "non-stop", "2 stops") into numerical values for model compatibility.  

## **Model Selection and Training**  
The dataset was split into training (80%) and testing (20%) sets. Several machine learning models were evaluated for their performance in predicting flight ticket prices.  

- **Linear Regression**: The initial model achieved an accuracy of **41%**, which indicated that a linear relationship was not sufficient for capturing complex patterns in the dataset.  

- **Stacking Regressor**: A more advanced ensemble learning approach, which combined multiple base models, improved the accuracy to **80%**.  

- **Random Forest Regressor**: The best-performing model, with **200 decision trees** and a maximum depth of **10**, resulted in an accuracy of **81%**, demonstrating its ability to capture nonlinear relationships and interactions between features.  

## **Conclusion**  
The project successfully developed a machine learning model for flight fare prediction. The **Random Forest Regressor** was identified as the most effective model, achieving an accuracy of **81%**, which is a significant improvement over linear regression. This model can be further enhanced by incorporating advanced techniques such as hyperparameter tuning, feature selection, and ensemble learning to further improve its predictive power.
