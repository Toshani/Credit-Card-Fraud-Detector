# Credit Card Fraud Detector - Mini Project (Special Topic, 3rd semester)

This is special topic project repository where we have implemented Credit Card Fraud Detection. 
We have used the kaggle data set and implemented LabelEncoder, SMOTE-ing and then KNN classifier.

# Dataset Description:
The dataset given to us was aready cleaned and ready for pre-processing, having the following features: 
1. Each record consists of 30 features including the details such as category, time, amount etc. 
2. Each record belongs to one of 2 classes, fraud or genuine
3. 250k+ examples in train and around 25k in test

Link to the original dataset: https://www.kaggle.com/mlg-ulb/creditcardfraud?select=creditcard.csv (Credit Card Fraud Detection)

# Libraries Used: 
Pandas, Numpy, Matplotlib, Seaborn, csv

# Steps:
1. Import all the libraries mentioned. Also import drive from google, and import/read the dataset. 
2. Perform data visualization to find out the state of the data - ready to use or pre-processing required. Use pie charts, bar graphs, histograms, heat maps etc. 
3. Pre-processing - Not required as we see that the datset is cleaned and ready to use. We see that there are 492 fraud entries and 284315 genuine entries. 
4. We see that the data is highly imabalanced as well as the fact that our dataset has sensitive information which means encoding is required. 
5. Apply LabelEncoder on the dataset from sklearn.preprocessing.
6. Split the dataset into train and test in the ratio 90:10.
7. Implement SMOTE-ing over the dataset in order to balance it and prevent over-fitting.
8. Train the model using KNeighborsClassifier. 

# Conclusions and Performance Metrics
* Accuracy: 0.9979284435237527
* Recall:  0.8333333333333334
* Precision:  0.43956043956043955
* F1 Score:  0.5755395683453238

We see that KNN model is not fit for classification in our data set even though it is a well proven algorithm. We are getting a very low precision and F1 score depicting that the training set fails to help classify the test set. As such, it would be better to try and experiment with models such as Random Forest and verify the same with k-fold cross validation.

# Acknowledgements
I'd like to thank Prof. Kakoli Bora for her guidance throughout the project. I'd also like to thank my partner - Vismaya G Iyer for her contribution in the project.

