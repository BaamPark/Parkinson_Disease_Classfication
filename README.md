# Parkinson_Disease_Classfication

## Dataset
The dataset contains speech recordings of 188 patients with Parkinson's disease and 64 healthy individuals. 
The recordings were collected by sustaining the phonation of the vowel /a/ with three repetitions. 
Various speech signal processing algorithms were applied to extract clinically useful information for Parkinson's disease assessment. 
The dataset is available from the UCI Machine Learning Repository and should be cited if used.

##Parkinson_EDA.ipynb
The file performs exploratory data analysis (EDA) on a dataset of Parkinson's disease classification. 
It is designed to visulaize as follows:
- class frequency
- PCA
- feature correlation using heatmap, boxplot, and pairplot

##PD_PCA_ML.ipynb
Several classification machine learning algorithms are used to classi to classify subjects as having Parkinson's disease or not. Logistic regression was used for performance evaluation on different dimensionality reduction methods, but it may not be effective for high dimensionality and non-linearity. Gaussian Naive Classifier, Random Forest Classifier, and Support Vector Machine were considered as they handle such problems. The Gaussian Naive Classifier uses Bayes theorem and independence between features to estimate the probability of a class. Random Forest is an ensemble of decision trees that can handle many features and resist overfitting, while SVM finds a hyperplane to separate classes and handles non-linearity and high dimensionality.

## Resources
- Parkinson's Disease Classification Data Set: https://archive.ics.uci.edu/ml/datasets/Parkinson%27s+Disease+Classification#
