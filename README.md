<h1> Dont-Overfit </h1>

<h2> Final Submission </h2>

The Final Submission of Dont Overfit! including all the codes complied in one Jupyter Notebook, Project Report and Presentation can be found in the [Final Code, Presentation and Report](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Final%20Code,%20Presentation%20and%20Report) directory.

<h2> Presentation Video Link </h2>

The Final Video Recording of the Presentation can be found [here](https://youtu.be/n1qj-ji7kr0).

<h2> Link to Problem Statement: </h2>

[https://www.kaggle.com/c/dont-overfit-ii/overview](https://www.kaggle.com/c/dont-overfit-ii/overview)

<h2> Link to Datasets: </h2>

[https://www.kaggle.com/c/dont-overfit-ii/data](https://www.kaggle.com/c/dont-overfit-ii/data)

The dataset for the project can also be found in the [Datasets](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Datasets) directory.

<h1> Process </h1>

<h2> 1: Literature Survey and Exploratory Data Analysis: </h2>

<h3> a: Literature Survey </h3>

The Literature Survey of this project can be found in the [Literature Survey](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Literature%20Survey) directory.

<h3> b: Exploratory Data Analysis </h3>

* Basic dataset analysis has been performed on the dataset in question. The mean and standard deviations of the feature have been computed and observed. These are no missing values in the dataset. Basically the dataset is as clean as it can be.

* A simple Logistic Regression classifier was fitted and tested on the dataset and provided 100% accuracy on the training data. However, when tested on the test data, the same model, produced an accuracy of 66.2%. This is a clear indicator of overfitting.

* Some analysis was performed on the features of the data to determine the most important features with respect to the target output. A correlogram was plotted and observed. The distributions of each feature was observed and found to be Gaussian and unimodal in nature.

* We know that the target value for each data point depends on the 300 features associated with it. However, since the origin of the data is unknown, there is a possibility that the data may be sequential i.e. the current row's target value can depend on the target value of the previous row. This possibility cannot be ignored as it will change the way we look at data henceforth. To verify the same the ACF and PACF plots were plotted for the target output. The results state unequivocally, that rows do not have autocorrelation. Hence we conclude that the data is not Sequential ion nature and the target values for each data point are independent of one another.

The detailed implementation and explaination of the Exploratory Data Analysis of this project can be found in the [Exploratory Data Analysis](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Exploratory%20Data%20Analysis) directory.

<h2> 2: Experimentation: </h2>

<h3> a: Selecting a Classification Model: </h3>

Let us try out a few Classification Models without any Dimensionality Reduction and select the best one for future experimentation.

<ol>
<li> Logistic Regression Classifier (Accuracy = 0.662) </li>
<li> Support Vector Classifier (Accuracy = 0.663) </li>
<li> Decision Tree Classifier (Accuracy = 0.568) </li>
<li> Gaussian Naive Bayes Classifier (Accuracy = 0.568) </li>
<li> Gaussian Process Classifier (Accuracy = 0.526) </li>
<li> Random Forest Classifier (Accuracy = 0.542) </li>
<li> AdaBoost Classifier (Accuracy = 0.542) </li>
<li> K Nearest Neighbours Classifier (Accuracy = 0.560) </li>
<li> Artificial Neural Network Classifier (Accuracy = 0.660) </li>
</ol>

Based on the accuracy result, implementation complexity and training time of the above Classification Models, we decided to move ahead using the Logistic Regression Classifier for our further experimentation.

<strong> NOTE: </strong> Python Implementation for the above Classification Models can be found in the [Classification Models](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Classification%20Models) directory.

<h3> b: Selecting a Dimensionality Reduction Technique: </h3>

Let us try out a few Dimensionality Reduction techniques to try and improve the accuracy of the result produced by the Logistic Regression Classifier.

<ol>
<li> Principle Component Analysis (Accuracy = 0.649) </li>
<li> Singular Value Decomposition (Accuracy = 0.724) </li>
<li> Lasso Regression (Accuracy = 0.848) </li>
</ol>

Based on the accuracy result and implementation complexity, Lasso Regression appears to be the best choice and the Results obtained by using Lasso Regression are satisfactory.

<strong> NOTE: </strong> Python Implementation for the above Dimensionality Reduction Techniques can be found in the [Dimensionality Reduction](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Dimensionality%20Reduction) directory.

<h1> Results </h1>

The Class Labels predicted by our various Machine Learning Models can be found in the [Class Labels Generated by Various Models](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Class%20Labels%20Generated%20by%20Various%20Models) directory.

The Screenshots of the Kaggle Test results can be found in the [Kaggle Test Result Screenshots](https://github.com/mayankagarwal44442/Dont-OverFit/tree/master/Kaggle%20Test%20Result%20Screenshots) directory.
