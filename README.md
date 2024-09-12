# svm-socialnetworkads
a Support Vector Machine (SVM) model is implemented and evaluated to address the classification problem of Social Network Ads. 
The aim is to determine whether a user would purchase a particular product based on a set of given features that describe the user. 
The features include user ID, gender, age, and estimated salary. 
We utilize the SVM algorithm that is known for its ability to handle both linear and nonlinear classification problems to classify whether a user would make a purchase of a
product or not.

The dataset used is Social Network Ads dataset from Kaggle. The dataset has
information about user’s ID, gender, age, estimated salary, and a column of
whether the user purchased the product or not.

SVMs are a powerful set of supervised learning methods used for classification,
regression and outliers’ detection, it is widely used for various tasks such as text
classification, image classification, spam detection, handwriting identification,
anomaly detection, etc. SVMs classify data by finding an optimal line or
hyperplane that maximizes the distance between each class in an N-dimensional
space, making them particularly effective for classification problems of high-
dimensional data and complex, nonlinear relationships.<br/>
Advantages:<br/>
• Effective in high dimensional spaces, SVMs perform well in cases
where the number of dimensions is high, making them suitable for
complex datasets.<br/>
• Effective in cases where number of dimensions is greater than the
number of samples.<br/>
• Only a subset of training points in the decision function called
support vectors are used, making SVMs memory efficient.<br/>
• Versatile; different Kernel functions can be specified for the
decision function, making SVMs adapt to different types of data and
problems. For this project, a linear kernel is appropriate given the
nature of the dataset. In addition, common kernels are provided,
but it is possible to specify custom kernels.

The model was evaluated with two scenarios:
Scenario 1. With the UserID Feature <br/>
Scenario 2. Without the UserID Feature <br/>

|                      |  With userID |  Without userID |
| :---                 |     :---:      |          ---: |
| **Validation Accuracy**  | 0.7875    | 0.825   |
| **Model Accuracy**       | 0.875       | 0.875     |

Confusion Matrix yielded the same result for both scenario:
[[43 2]
[ 8 27]]
![Unknown](https://github.com/user-attachments/assets/5c444300-8a9d-4913-89de-614edddac438)

The model achieved an accuracy of 87.5% on the test set indicating strong overall performance. The confusion matrix shows 43 true negatives, 27 true positives, 2 false positives, and 8 false negatives suggesting the model is more accurate at predicting non-purchases.
