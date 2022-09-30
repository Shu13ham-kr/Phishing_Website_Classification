# Phishing_Website_Classification
A Machine Learning model to classify wether a website is a phishing website or not using Python (Jupyter Notebbok).

Result :
**Testing accuracy = 93.70%
Training accuracy = 94.55%**

Libraries used:
**pandas,
numpy,
seaborn,
matplotlib.pyplot,
from sklearn.model_selection : train_test_split,
from sklearn.preprocessing : StandardScaler,
from sklearn.linear_model : LogisticRegression,
from sklearn.metrics : accuracy_score**

Approach:
1. First we import the required libraries and then we use pandas to read the csv file.
2. The data is already cleaned so we dont need to do much in pre-processing but I still checked for null values and outliers.
3. Then I checked the correlation of all the features to remove the unwanted features.
4. Then I visually represented the correlations of the remaining features using heatmap.
5. Then I stored the target variable in y and the features required to predict it in x.
6. Using the train_test_split library I split x and y into training and testing sets with testing set being 20% of the original.
7. Next I used StandardScaler to scale the data in a standard range (though it wasn't neccessary in this data set as all the values are only -1, 0, 1).
8. Since we had to classify wether a website is phishing website or not I used logistic regression for classification (as linear regression is used when target variable is linearly dependent on the independent variables and continous).
9. We can then use the accuracy_score library or .score() method to check the accuracy of our model.
10. At last I presented a bar graph to represent the predicted result.
