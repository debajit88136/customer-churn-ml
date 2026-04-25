# customer-churn-ml
Customer churn prediction using machine learning (Random Forest, feature engineering, and model tuning)
Customer Churn Prediction (Machine Learning Project)

This project focuses on predicting whether a customer is likely to leave a service (churn) or not. The goal is to help businesses identify at-risk customers early so they can take action to retain them.

Dataset
The project uses the Telco Customer Churn dataset, which contains around 7000 customer records. It includes information such as customer tenure, billing details, contract type, and service usage.

What I did in this project

* Cleaned the data by handling missing values in the TotalCharges column
* Converted data types and removed unnecessary columns like customerID
* Encoded categorical variables to make the data suitable for machine learning
* Built a Random Forest model to predict churn
* Evaluated the model using accuracy, confusion matrix, and classification report

Model improvement

Initially, the model had good accuracy (~79%) but was not detecting churn customers well (recall was low).

To improve this:

* Applied class_weight to handle imbalance
* Adjusted prediction threshold from 0.5 to 0.3

Final result

* Accuracy: ~75%
* Churn recall improved from 45% to 73%

This means the model is now much better at identifying customers who are likely to leave, which is more important from a business perspective.

Key insights

* Customers with shorter tenure are more likely to churn
* Higher monthly charges increase churn probability
* Long-term contracts reduce churn
* Payment methods like electronic check are associated with higher churn

Tools used

Python, Pandas, NumPy, Scikit-learn, Google Colab

Conclusion

This project shows how machine learning can be applied to a real business problem. Instead of focusing only on accuracy, the model was improved based on business needs (detecting churn customers), which makes it more practical and useful.

Future improvements

Future Improvements

* Try more advanced models like XGBoost or LightGBM
* Perform proper hyperparameter tuning for better performance
* Deploy the model as a simple web app using Streamlit
* Use more real-world data for better generalization

