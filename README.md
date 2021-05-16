# Logistic-Regression

Used the Heart Disease Dataset from kaggle to predict if a person has heart Disease or not.
https://www.kaggle.com/ronitf/heart-disease-uci
The data set contains following columns:
-age
-sex
-chest pain type (4 values)
-resting blood pressure
-serum cholestoral in mg/dl
-fasting blood sugar > 120 mg/dl
-resting electrocardiographic results (values 0,1,2)
-maximum heart rate achieved
-exercise induced angina
-oldpeak = ST depression induced by exercise relative to rest
-the slope of the peak exercise ST segment
-number of major vessels (0-3) colored by flourosopy
-thal: 3 = normal; 6 = fixed defect; 7 = reversable defect

## Workflow
- Trained the model using GLM method of Logistic Regression and calculated the disease probabilities
- Probabilities above 0.5 were put in the category of diseased(1) and others non diseased(0)
- Created a confusion matrix and calculated accuracy of the model
- Calculated other parameters like sensitivity and specificity
- Also constructed a ROC curve, the area under the curve came about 92%, which tells that the test is pretty much accurate
- Finding the optimal cutoff point
  - Took cutoff values from 0.0 to 0.9 to find where the sensitivity and specificity gert balanced
  - Repeated the above procedures 
