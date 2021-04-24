# Credit_Risk_Analysis
## Purpose
The purpose of this assignment is to use machine learning to solve real word challenges, in this case a challenge about credit card risk. To do this we needed to first use the imbalanced-learn and scikit-learn libraries to build and evaluate models by using oversampling, under sampling and the SMOTEENN algorithm which is a combination of over and under sampling, to predict credit risk.
## Results
### Naive Random Oversampling
•	Balanced Accuracy Score: 0.6494575410534504

•	Precision Scores
    
    o	High Risk: 0.01
    o	Low Risk: 1.00
    o	Average: 0.99

•	Recall Scores
    
    o	High Risk: 0.73
    o	Low Risk: 0.57
    o	Average: 0.57

![image](https://user-images.githubusercontent.com/76131315/115972681-d4566b00-a51d-11eb-8e3d-9e86ab267a61.png)


### SMOTE Oversampling
•	Balanced Accuracy Score: 0.6584476794265021

•	Precision Scores

    o	High Risk: 0.01
    o	Low Risk: 1.00
    o	Average: 0.99

•	Recall Scores

    o	High Risk: 0.63
    o	Low Risk: 0.68
    o	Average:  0.68

![image](https://user-images.githubusercontent.com/76131315/115972709-fea82880-a51d-11eb-8cda-250119e89dcc.png)

### Undersampling using ClusterCentroids
•	Balanced Accuracy Score: 0.5447339051023905 

•	Precision Scores

    o	High Risk: 0.01
    o	Low Risk: 1.00
    o	Average: 0.99

•	Recall Scores

    o	High Risk: 0.69
    o	Low Risk: 0.40
    o	Average: 0.40

![image](https://user-images.githubusercontent.com/76131315/115972732-1da6ba80-a51e-11eb-8a55-8bb5e81a962b.png)

### SMOTEENN Combination Sampling
•	Balanced Accuracy Score: 0.6484827242078745

•	Precision Scores

    o	High Risk: 0.01
    o	Low Risk: 1.00
    o	Average: 0.99

•	Recall Scores

    o	High Risk: 0.72
    o	Low Risk: 0.57
    o	Average: 0.58

![image](https://user-images.githubusercontent.com/76131315/115972742-357e3e80-a51e-11eb-9478-e629a55af1da.png)

### Balanced Random Forest Classifier
•	Balanced Accuracy Score: 0.7885466545953005

•	Precision Scores

    o	High Risk: 0.03
    o	Low Risk: 1.00
    o	Average: 0.99

•	Recall Scores

    o	High Risk: 0.70
    o	Low Risk: 0.87
    o	Average: 0.87

![image](https://user-images.githubusercontent.com/76131315/115972763-4dee5900-a51e-11eb-9ab6-056d31d1ce46.png)

### Easy Ensemble AdaBoost Classifier
•	Balanced Accuracy Score:  0.9316600714093861

•	Precision Scores

    o	High Risk: 0.09
    o	Low Risk: 1.00
    o	Average: 0.99

•	Recall Scores
    
    o	High Risk: 0.92
    o	Low Risk: 0.94
    o	Average: 0.94

![image](https://user-images.githubusercontent.com/76131315/115972778-6a8a9100-a51e-11eb-8ffc-823b8f35487c.png)

## Summary
When looking at the Balanced Accuracy Scores we can see that the AdaBoost model has the highest accuracy at 93.17% then it is Random Forest at 78.85% then the scores become a lot similar with SMOTE having 65.85%, then Naïve Random having 64.95% and SMOTEENN having 64.85% and finally in last place is the Undersampling using ClusterCentroids have 54.47% accuracy. For Precision scores, every model had the same low risk score at 1.00 as well the same average at .99 but AdaBoost has the highest High-Risk score at 0.09 while Random Forest has a High-Risk score of 0.03. The rest have a High-Risk score of 0.01. For Recall scores, AdaBoost is once again the highest with a scores of 0.94 and 0.92, and Random Forest is second for the average and Low Risk at 0.87, its High Risk is at 0.70 which is fourth to Naïve Randoms 0.73 High Risk score and SMOTEENN’s 0.72 High Risk score.  The Naïve Randoms model has an Average score and Low-Risk score of 0.57, the SMOTEENN model has an Average score of 0.58 and a Low-Risk score of 0.57. The Undersampling model has an Average and Low-Risk score of 0.40 and a High-Risk score of 0.69 while the SMOTE model has a High-Risk recall score of 0.63 and an Average and Low-Risk score of 0.68. When Looking at these numbers it is easy to recommend the AdaBoost model because of its high accuracy score (with it being in the 90s) and also its high Recall scores (with the lowest being 0.92) not only are these numbers high but they are the highest when compared to all the models and therefore the AdaBoost Model should be the one used. 

