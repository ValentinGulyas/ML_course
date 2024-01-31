![image](https://github.com/ValentinGulyas/ML_course/assets/144483901/bf5aa18f-9c87-4a0f-aa70-0fa31d047a22)# ML_course
**------------------------------------------------------------------------------**
CA01

The CA01_Team_Code was generated by me (Valentin), Lindsay, and Andrea.
The code performs Exploratory Data Analysis (EDA) with the goal of preparing the data for an ML model that will predict house prices.

**------------------------------------------------------------------------------**
**CA02**

**Objective:** The objective of the code is to predict whether an email is (i) spam or (ii) not spam.

**Overview:** Our objective is a Natural Language Processing (NLP) task, which falls under the classification type of ML since it focuses on language and text. The classification pre-processes in NLP must convert the text to zero and one’s as well as a dictionary (or bag-of-words) as a vector or matrix, which is performed by our code. Once the pre-processing is complete, the data is split. The training data consists of features (i.e., features_matrix) and a target (e.g., labels). A model is then generated from the trained data (e.g., pred), which is compared to the testing dataset (i.e., test_labels). The code runs a comparison analysis that results in an accuracy score, which is then further visualized by a confusion matrix.

**Libraries**
There are 5 packages we need to import:
1. os
2. numpy
3. Counter from collections
4. GaussianNB from sklearn.naive_bayes
5. accuracy_score from sklearn.metrics

**Breakdown of each package:**
1. os library enables us to use operating system (hence os) dependent functionality. It allows us to edit paths and navigate file/directory operations.
    Documentation: https://docs.python.org/3/library/os.html

2. numpy is an array-processing package that is widely accepted as the most used scientific computing package in python
    Documentation: https://numpy.org/
    
3. Counter is a module from collections, and acts as a subclass of dictionaries. It allows us to count - and keep track of - elements by storing each element as a key in a key-value pair whilst storing the count of the element as a pair.
    Article: https://www.digitalocean.com/community/tutorials/python-counter-python-collections-counter
    
4. Naive-Bayes (NB) and conditional probability assumes normal (or gaussian) distributions. The GaussianNB module allows us to fit a Gaussian NB according to x (i.e., IVs/features/columns) and y (i.e., DV/target/predictor), using the .fit() function. Moreover, this module enables us to perform a classification on an array of test vectors with the .predict() function.
    https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html
    
5. The accuracy_score module from sklearn.metrics computes the model's accuracy. It either returns the fraction (its default setting) or the count of correct prediction, which can be applied with the (Normalized = False) statement. Lastly, this module allows us to calculate and display a confusion matrix with the confusion_matrix() command, which evaluates the accuracy of a classification.
    Documentation: https://scikit-learn.org/stable/modules/model_evaluation.html

6. The pandas library is needed, if we want to display the confusion matrix a good-looking table for readability. We do this by converting the confusion matrix into a pandas df, and then display it.

**Our strategic approach is as follows:**
1.	Acquire the data
2.	Pre-process the data
    a.	Open each file (i.e., email)
    b.	Tokenization of words (generate bag-of-words)
3.	Split the data
    a.	X_train + y_train (e.g., 80% of the entire dataset)
    b.	X_test + y_test (e.g., 20% of the entire dataset)
4.	Instantiate a classifier
5.	Fit the classifier to the training data (i.e., X_train and y_train)
6.	Generate predicted tags (i.e., X_test)
7.	Calculate an accuracy score (i.e., y_test, y_pred)
    a.	Visualize the accuracy with a confusion matrix 
![image](https://github.com/ValentinGulyas/ML_course/assets/144483901/3471ca38-a45c-4230-8dd6-b27634ca2040)


Repository for my ML course
