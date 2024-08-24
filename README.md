# Heart Disease Prediction
Heart or cardiovascular diseases (CVDs) affect the heart and blood vessels, impacting overall health. Early detection and management are vital for better outcomes. Machine learning and predictive models have recently become key tools in identifying heart disease risk. These models analyze patient data, such as medical history and lifestyle, to predict the likelihood of developing heart disease. This technology helps healthcare providers make informed decisions, allowing for earlier intervention and personalized treatment, ultimately reducing the impact of heart diseases and saving lives.<br>
**Objective**: Our primary objective is to ascertain the probability of an individual being susceptible to a severe heart problem based on some features. <br>
**Methods Used**: Exploratory Data Analysis, Inferential Statistics, Data Visualization, Machine Learning, Predictive Modeling.<br>
**Language, Libraries, technologies used**: Python, Pandas, Matplotlib, Seaborn, Numpy, Scipy, Scikit-learn.<br>
## DATA DICTIONNARY 

1. age: age in years
2. sex: sex
    - 1 = male
    - 0 = female
3. cp: chest pain type
     - Value 0: typical angina
     - Value 1: atypical angina
     - Value 2: non-anginal pain
     - Value 3: asymptomatic
4. trestbps: resting blood pressure (in mm Hg on admission to the hospital)
5. chol: serum cholestoral in mg/dl
6. fbs: (fasting blood sugar > 120 mg/dl)
    - 1 = true;
    - 0 = false
7. restecg: resting electrocardiographic results
    - Value 0: normal
    - Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
    - Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
8. thalach: maximum heart rate achieved
9. exang: exercise induced angina
    - 1 = yes
    - 0 = no
10. oldpeak = ST depression induced by exercise relative to rest
11. slp: the slope of the peak exercise ST segment
    - Value 0: upsloping
    - Value 1: flat
    - Value 2: downsloping
12. caa: number of major vessels (0-3) colored by flourosopy
13. thal:
    - 0 = error (in the original dataset 0 maps to NaN's)
    - 1 = fixed defect
    - 2 = normal
    - 3 = reversable defect
14. output (the lable):
    - 0 = no disease,
    - 1 = disease

## Key Insights 
- 54.3% of cases in the dataset are classified as heart disease against 44.7% and 68.2% are male
- There is no difference in serum cholesterol, fasting blood sugar, resting electrocardiographic results between those who have heart disease and those who don't in the dataset
- Those with 0 major vessels are at higher risk of heart disease and, those with typical angina are at less risk of heart disease in this dataset
- Svm was the best model with an accuracy_score of 0.89 , a precison_score of 0.90 a recall_score of 0.88 and a f1_score of 0.90
- chest pain type (cp), the slope of the peak exercise ST segment (slp) , resting electrocardiographic results (restecg), sex and number of major vessels (0-3) colored by flourosopy (caa) were the three most important features for the model
