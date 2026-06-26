# Logistic Regression – Airline Customer Satisfaction Prediction

## Project Overview

This project applies Logistic Regression using Scikit-learn to predict airline passenger satisfaction based on customer survey data. The workflow includes data preprocessing, categorical variable encoding, train-test splitting, model training, performance evaluation, and interpretation of factors influencing customer satisfaction.

## Dataset

The dataset contains passenger demographics, travel information, service quality ratings, and flight delay metrics. The target variable is **satisfaction**, classified as either **Satisfied** or **Dissatisfied**.

## Methodology

* Performed data cleaning and missing value treatment.
* Encoded categorical variables for machine learning compatibility.
* Split the dataset into training (80%) and testing (20%) sets using stratified sampling.
* Standardized predictor variables using StandardScaler.
* Documented the assumptions of the Logistic Regression model.
* Trained a Binomial Logistic Regression model to predict customer satisfaction probabilities.
* Evaluated model performance using a Confusion Matrix, Precision, Recall, F1-score, and Classification Report.
* Interpreted model coefficients, discussed limitations, and proposed recommendations for future improvements.

## Logistic Regression Assumptions
The target variable is binary (Satisfied or Dissatisfied).
Observations are assumed to be independent.
Categorical variables were encoded into numerical features using one-hot encoding.
Missing values were handled prior to model training.
Continuous features were standardized to improve model convergence.
Logistic Regression assumes a linear relationship between continuous predictors and the log-odds of the outcome. This assumption was acknowledged but not formally tested in this project.


## Model Performance

Confusion Matrix

| Actual / Predicted | Dissatisfied | Satisfied |
|-------------------|-------------:|-----------:|
| Dissatisfied | 9546 | 2213 |
| Satisfied | 2232 | 11985 |

| Metric | Score |
|----------|---------:|
| Accuracy | 83% |
| Precision | 84.4% |
| Recall | 84.3% |
| F1-Score | 84.3% |

The Logistic Regression model achieved an accuracy of 83%, with precision (84.4%), recall (84.3%), and an F1-score of 84.3%, indicating a good balance between correctly identifying satisfied passengers and minimizing false classifications.
Overall, The model demonstrated balanced predictive performance, effectively identifying satisfied passengers while maintaining a balanced trade-off between false positives and false negatives.

## Key Drivers of Customer Satisfaction

### Positive Drivers

* Inflight Entertainment
* Seat Comfort
* On-board Service
* Check-in Service
* Ease of Online Booking
* Leg Room Service

### Negative Drivers

* Disloyal Customer Status
* Economy Class Travel
* Personal Travel
* Arrival Delays
* Food and Drink Satisfaction
* Departure/Arrival Time Convenience

Inflight Entertainment was identified as the strongest positive predictor of customer satisfaction, while being a Disloyal Customer was the strongest negative predictor.

## Business Recommendations

* Invest in enhancing inflight entertainment offerings to improve passenger experience.
* Improve seat comfort, leg room, and on-board service quality.
* Streamline the online booking and check-in processes.
* Reduce operational delays and improve delay communication.
* Strengthen customer loyalty programs to improve retention and satisfaction.
* Enhance the travel experience for Economy Class passengers through targeted service improvements.

## Limitations

* Logistic Regression assumes a linear relationship between predictors and the log-odds of satisfaction.
* The analysis is limited to variables available in the dataset and may not capture all factors affecting customer satisfaction.
* Results indicate associations rather than direct causal relationships.

## Future Improvements

* Compare performance with advanced machine learning models such as Random Forest, XGBoost, and Gradient Boosting.
* Incorporate additional operational and customer behavior variables.
* Deploy the model within customer experience systems for real-time satisfaction prediction and proactive service recovery.

## Technologies

* Python
* Jupyter Notebook
* Google Colab
* Git
* GitHub

## Python Libraries

* Pandas
* NumPy
* Scikit-learn
* Matplotlib
## Repository Contents

* `logistic_regression_analysis.ipynb` – Complete analysis and model development notebook.
* `README.md` – Project summary, methodology, results, and business recommendations.
