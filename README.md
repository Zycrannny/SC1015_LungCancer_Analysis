# This is lung cancer dataset guide on our project

## About
This is our Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) revolving around the common indicators of lung cancer. The dataset is taken from [Kaggle]([https://www.kaggle.com/datasets/thedevastator/cancer-patients-and-air-pollution-a-new-link).

## Contributors
Ho King Hei, Fong Jian Yuan, Heng Ziyang

## Problem definition
Given the alarming statistics surrounding lung cancer, particularly its status as the leading cause of cancer death worldwide, there is an urgent need for further understanding and identification of risk factors that contribute to its development.
-How can we predict if a person has lung cancer? If possible, what stage?
-Which model is the best to predict the above?

## Models used
-Support Vector Machine (SVM) model
-Random Forest model

## Data extraction
- Import data from .csv file obtained from Kaggle
- Cleaning dataset by replacing arbitrary alphabets to meaningful numbers for easier manipulation, as well as removing irrelevant data
- Ensuring no empty or missing values

## Data visualisation
- In this section, we explore the data using boxplot to detect for any outliers
- Using correlation matrix, we can see the correlation values of the various features and the cancer result

## Machine Learning
- We train the two models, random forest and SVM to attempt to accurately predict the lung cancer and severity of it within a target
- Models are then examined using mean accuracy, standard deviation as well as k-fold cross validation
- Random forest has an accuracy of 1.00 on the test dataset, hence we are inclinely to rely on SVM due to a known failure rate on it

## Conclusion
- With random forest, we have managed to ascertain what were the specific factors that were highly indicative of one having a certain stage of lung cancer, and which were not as reliable.
- With SVM, we managed to relatively accurately predict the certain stages of lung cancer using the dataset we split to train it, as well as test it.
- Using the dataset, we have managed to obtain the top 3 common occurences for all patients that have lung cancer, as well as top 3 per severity

## Future Improvement
- Using a larger amount of datasets would certainly help to make our model grow and become even better at predicting
- In addition to the above, random forest might be reliable as it faces some errors, but is more accurate than SVM, to which we are not sure of as of now
- Work with real-world healthcare professionals and governments to gain access to datasets containing even more factors, which might have an even more common occurence than the ones we have discovered

## Learning points
- Usage of models not learned in SC1015 course such as Support Vector Machine (SVM) and Random Forest Model
- Evaluating accuracy of models -> Plotting confusion matrix and calculating the precision and accuracy 
- Sorting and ranking variables using feature importance to better understand the features in our data

## References
- <https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html>
- <https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html>
- <https://scikit-learn.org/stable/auto_examples/ensemble/plot_forest_importances.html#:~:text=Feature%20importances%20are%20provided%20by,impurity%20decrease%20within%20each%20tree.&text=Impurity%2Dbased%20feature%20importances%20can,features%20(many%20unique%20values).>
