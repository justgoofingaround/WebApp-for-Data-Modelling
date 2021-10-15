# Cool Science: A webapp for Data Modelling #

Project - 2 <br>
UCS757 - Building Innovative Systems <br>

## Overview: ##
Data Science webapp to show some of the capabilities of Flask and libraries such as sklearn, pandas, matplotlib, seaborn.

## Capabilities:

### Dataset upload
The webapp supports:
- CSV (delimiter: ',')
- TXT (delitimer: tab)

### Dataset summary
This page will show:
- 5 first rows to see the general aspect of the dataset.
- Statistical summary of each column.

### Preprocessing
We can create a new dataset (it will be saved as CSV) with the following options:

Feature selection:
- Automatic selection based on Chi-Squared estimator (the name will be created depending of the chosen parameters):
  - Number of features
  - Response variable
- Manual selection:
  - Name of the new dataset
  - Variables selection

Null values and columns with a unique value:
- Drop rows with null values:
  - Null in ALL columns
  - Null in ANY column
  - Never
- Drop variables with a unique value:
  - Yes
  - No
  
* Extra preprocessing (normalization, dummy variables...) will be done in model and predict steps.

### Graphs
Available visualizations for the chosen variables:

- Histograms
- BoxPlots
- Correlation plots

### Models
Models for Classification and Regression tasks.
It does not support multiclass classification at this moment (extra code to manage some metrics and graphs)

Available Algorithms:
- Logistic Regression (Classification)
- Linear Regression (Regression)
- Random Forests (both)
- K Nearest Neighbors (both)
- AdaBoost (both)
- Extreme Gradient Boosting (both)
- MultiLayer Perceptron (both)

K-Fold Cross-Validation (3, 5, 10)

Standard Scaling (Yes, No)

Manual Feature Selection

Classification Tasks Output:
- Fit time
- Score time
- Precision (Test and Train)
- Recall (Test and Train)
- F1 score (Test and Train)
- Accuracy (Test and Train)
- ROC AUC (Test and Train)
- ROC curves plot

Regression Tasks Output:
- Fit time
- Score time
- Explained Variance (Test and Train)
- R2 (Test and Train)
- Mean Squared Error (Test and Train)
- Measured vs Predicted values plot

### Predictions
Model building (with the complete dataset) and prediction for a set of introduced values.
The model will only include the variables with an introduced value.
The available algorithms are the same that were mentioned in "Models".
It also supports multiclass problems.


### Live Link: https://datamodelling.herokuapp.com/ ###
(Sample Data already enclosed in this github-repo)

### I/O Screenshot :<br/> ###
Output-1
![o1](https://user-images.githubusercontent.com/43958244/137478758-972be20e-e829-42fd-8a1e-76de3559c1f8.png)
<br>
<br>
Output-2
![o2](https://user-images.githubusercontent.com/43958244/137478821-8d29517d-0a22-4af7-ae30-280026653c5b.png)
</br>
Output-3
![o3](https://user-images.githubusercontent.com/43958244/137478884-1cacacdb-5145-4bc8-ab4f-e358bf6bc62f.png)
<br>
<br>
Output-4
![o4](https://user-images.githubusercontent.com/43958244/137478915-2f3fdbb8-6ecd-4d80-8623-71831394d2ba.png)
</br>

### Novelty :<br/> ###
-	This web-app provides aid for the user to perform the Data Modelling operations without having trouble to write code from scartch for the same.<br>

- With help of this web-app the user will be able to upload his own dataset or can use the previous uploaded datset, perform data preprocessing, summarize dataset, analyse data with the help of various types of graphs, can perform modelling using various alogrithm and finally can predict from the applied model. <br>
