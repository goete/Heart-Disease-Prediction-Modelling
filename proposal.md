Title

# Introduction:
* Provide some relevant background information on the topic so that someone unfamiliar with it will be prepared to understand the rest of your proposal
* Clearly state the question you will try to answer with your project
* Identify and describe the dataset that will be used to answer the question

# Preliminary exploratory data analysis:
* Demonstrate that the dataset can be read from the web into R 
* Clean and wrangle your data into a tidy format
* Using only training data, summarize the data in at least one table (this is exploratory data analysis). An example of a useful table could be one that reports the number of observations in each class, the means of the predictor variables you plan to use in your analysis and how many rows have missing data. 
* Using only training data, visualize the data with at least one plot relevant to the analysis you plan to do (this is exploratory data analysis). An example of a useful visualization could be one that compares the distributions of each of the predictor variables you plan to use in your analysis.

# Methods:
* Explain how you will conduct either your data analysis and which variables/columns you will use. Note - you do not need to use all variables/columns that exist in the raw data set. In fact, that's often not a good idea. For each variable think: is this a useful variable for prediction?

14 important variables:
1. #3  (age)       
2. #4  (sex)
3. #9  (cp) chest pain type (categorical)        
4. #10 (trestbps)  - resting blood pressure
5. #12 (chol)      - cholesterol level
6. #16 (fbs)       - fasting blood sugar
7. #19 (restecg)   - ecg results
8. #32 (thalach)   - maximum heart achieved
9. #38 (exang)     - exercise induced angina
10. #40 (oldpeak)  - ST depression induced by exercise relative to rest
11. #41 (slope)     - the slope of the peak exercise ST segment
        -- Value 1: upsloping
        -- Value 2: flat
        -- Value 3: downsloping
12. #44 (ca)     number of major vessels (0-3) colored by flourosopy   
13. #51 (thal)      3 = normal; 6 = fixed defect; 7 = reversable defect
14. #58 (num)       (the predicted attribute 0 or 1)

* Describe at least one way that you will visualize the results

# Expected outcomes and significance:
* What do you expect to find?
* What impact could such findings have?
* What future questions could this lead to?