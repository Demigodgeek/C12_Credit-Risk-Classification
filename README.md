# Credit Risk Classification
---

## About The Project

This project uses a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. 
This project uses various techniques to train and evaluate models with imbalanced classes:
+ Split the Data into Training and Testing Sets
+ Create a Logistic Regression Model with the Original Data
+ Predict a Logistic Regression Model with Resampled Training Data
+ Write a Credit Risk Analysis Report
 
---

## Installation

This project leverages python 3.9 with the following packages:

+ Pandas 
+ Numpy
+ Scikit-learn
+ Imbalanced-learn

### Installation Guide(MacOS & Windows)

1.  Open a terminal or command prompt on your computer.
2.  Install all packages by running the commands: 

```bash
  pip install pandas 
  pip install numpy
  pip install scikit-learn
  pip install imbalanced-learn
```
---

## Summary

This code uses a logistic regression model to predict loan status based on a set of features. The dataset used contains information about loans, including the loan status (0 for a healthy loan, 1 for a high-risk loan) and various features such as the loan amount, interest rate, and employment status of the borrower.

The code first reads the data from a CSV file and separates the features (X) and the labels (y). The data is then split into training and testing sets using the train_test_split function from the Scikit-learn library. A logistic regression model is then instantiated with a random_state parameter set to 1, and is fit to the training data.

The model is then used to make predictions on the testing data, and various metrics are calculated to evaluate the performance of the model. These metrics include the balanced accuracy score, confusion matrix, and classification report.

The code is then repeated, but this time the training data is resampled using the RandomOverSampler function from the imbalanced-learn library. The model is again fit to the resampled training data, and the performance metrics are calculated using the testing data.

The results of both models are compared, and it is shown that the resampled model performs better in terms of its ability to predict high-risk loans (label 1).

---

## Contributor
* Demi Gao
---

## License
This program is licensed under the MIT License.