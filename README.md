# predict_hazard_score_of_houses
Predict the hazardous score of a house based on the various features of the house.
Background/history
A Fortune 100 company, Liberty Mutual Insurance has provided a wide range of insurance products and services designed to meet their customers' ever-changing needs for over 100 years.
To ensure that Liberty Mutual’s portfolio of home insurance policies aligns with their business goals, many newly insured properties receive a home inspection. These inspections review the condition of key attributes of the property, including things like the foundation, roof, windows and siding. The results of an inspection help Liberty Mutual determine if the property is one they want to insure.
In this challenge, my task is to predict a transformed count of hazards or pre-existing damages using a dataset of property information. This will enable Liberty Mutual to more accurately identify high risk homes that require additional examination to confirm their insurability.
Data Explanation (Data Prep/Data Dictionary)
Two datasets are available in the Kaggle challenge:
•	train.csv - the training set, contains the Hazard and anonymized predictor variables
•	test.csv - the test set, contains only the anonymized predictor variables
Each row in the dataset corresponds to a property that was inspected and given a hazard score ("Hazard"). We can think of the hazard score as a continuous number that represents the condition of the property as determined by the inspection. Some inspection hazards are major and contribute more to the total score, while some are minor and contribute less. The total score for a property is the sum of the individual hazards.

train.csv contains 
ID: This uniquely identifies each house
Hazard: This is the hazardous score for each house
T1_V1 to T2_V15 :There are 32 attributes , they are anonymized variables which are available before an inspection is ordered.
test.csv contains 
ID: This uniquely identifies each house
T1_V1 to T2_V15 :There are 32 attributes , they are anonymized variables which are available before an inspection is ordered.
Goal is to calculate Hazard score.
Data Preparation:
Dataset provided looks clean with around 100,000+ rows. Attributes are anonymized to ensure data privacy and to remove bias of any kind. 
Performed below checks in the data:
1.	Skewness check: Checked skewness in the data for each attributes.—>Looks good, none of the attribute has skewness.
2.	Data completeness Check: Checked if attributes has Null,None values. Removed Null if any.
3.	One hot encoding: Performed one hot encoding for categorical attributes to convert to numeric.
