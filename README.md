# breast_cancer_classification
This project uses the breast cancer dataset from sklearn library. 
Classification and Logistic Regression is used to predict and evaluate the data.
Here, the logistic regression model is used to evaluate the percentage of correct predictions.
The dataset is loaded into the dataframe in which, the 'Target' column is defined. It has the value 1
if the cancer is benign or 0 if the cancer is malignant. Now, with the model that we have,
cancer for any new data is classified into benign or malignant.

Dataset:
	The dataset is imported from sklearn dataset. With 570 instances and 32 features,
this dataset provides the sufficient data to classify any other new data about cancer into 
benign or malignant. The data that is imported isn't used directly, instead, the data imported
is loaded into a data frame using DataFrame() function in pandas library.

EDA:
	Here, the target column is defined. Like said before, 0 means the cancer is malignant
and 1 if the cancer is benign. The dataset is checked for any null or sentinel
values and there is none. Then, the mean is found for each and every feature with respect to the target value.
Now, the target column is isolated, every other feature other than feature is stored in X
and the target column is stored in Y.

Model Fitting:
	Here, the model is fit into test and train data. 20% of the data is used as test data.
The model is a Logistic Regression Model. Then, the result of the X_train data is predicted (0 or 1)
and the predicted data is checked with the Y_train data (target data). The accuracy score on
training data is around 95%. The same is done for the test data and the accuracy is around 93%.

Predicting:
	Input data is given within the code and can be changed if needed. This input data is
from Kaggle. After converting the input into numpy array, the prediction is done with respect to the model
and it is shown if the breast cancer is malignant or benign.
