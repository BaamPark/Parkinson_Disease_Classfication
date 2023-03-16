# Parkinson_Disease_Classfication

## Dataset
The dataset contains speech recordings of 188 patients with Parkinson's disease and 64 healthy individuals. 
The recordings were collected by sustaining the phonation of the vowel /a/ with three repetitions. 
Various speech signal processing algorithms were applied to extract clinically useful information for Parkinson's disease assessment. 
The dataset is available from the UCI Machine Learning Repository and should be cited if used.

## Parkinson_EDA.ipynb
The file performs exploratory data analysis (EDA) on a dataset of Parkinson's disease classification. 
It is designed to visulaize as follows:
- class frequency
- PCA
- feature correlation using heatmap, boxplot, and pairplot

## PD_PCA_ML.ipynb
Several classification machine learning algorithms are used to classi to classify subjects as having Parkinson's disease or not. Logistic regression was used for performance evaluation on different dimensionality reduction methods, but it may not be effective for high dimensionality and non-linearity. Gaussian Naive Classifier, Random Forest Classifier, and Support Vector Machine were considered as they handle such problems. The Gaussian Naive Classifier uses Bayes theorem and independence between features to estimate the probability of a class. Random Forest is an ensemble of decision trees that can handle many features and resist overfitting, while SVM finds a hyperplane to separate classes and handles non-linearity and high dimensionality. SMOTE upsampling method is used to address class imbalance problem. In conclusion, the combination of SMOTE, SVM, and PCA shows the best performance

## VAN.ipynb
This file implement variational autoencoder to address dimension reduction. 
VAE is a type of deep learning model used for unsupervised learning and dimensionality reduction, comprising an encoder and a decoder network. The encoder network maps input data to a lower-dimensional representation, while the decoder network maps the encoding back to the original input data. The VAE is trained to minimize the difference between the input data and the reconstructed data while maximizing the likelihood of the data given the latent representation. The ultimate goal of the VAE is to learn a probability distribution over the latent space, which can be used to generate new data points. However, the result shows that VAN doesn't outperform simple PCA with logistic regression.

## Kernel_PCA.ipynb
Kernel PCA is non-linear extension of PCA that serves for the same purpose. The kernel PCA maps the data into higher-dimensional feature space using kernel function to capture complex patterns and structure in the data that may not be captured by PCA. However, it doesn't outperform PCA with logistic regression. 

## Resources
- Parkinson's Disease Classification Data Set: https://archive.ics.uci.edu/ml/datasets/Parkinson%27s+Disease+Classification#
