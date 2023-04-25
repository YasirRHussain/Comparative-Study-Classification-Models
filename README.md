*** INTRODUCTION ***

Machine learning has become a crucial component in modern data analysis and decision-making. Selecting the best machine learning model for a specific task can be challenging, and to address this problem, I conducted an experiment using two popular datasets, Adult and CIFAR10. 

I tested these datasets on ten different machine learning models, focusing on each model's performance when presented with varying densities, types, and features of the data. 

This experiment aimed to gain insights into the strengths and weaknesses of each model and to determine the most suitable model for different data types and applications. 

The results of this experiment will provide valuable information to guide future selection of machine learning models.

*** INFORMATION ABOUT DATASETS ***

This section will list out the datasets used for the project.

Adult Dataset

CIFAR-10 Dataset

*** MODELS IMPLEMENTED ***

This section will list out all the machine learning classification models we have used for our project.

1. Logistic Regression
2. SVM
3. Naive Bayes
4. Random Forest
5. KNN Classifier
6. Ada Boost
7. SGD Classifier
8. MLP
9. LSTM
10.CNN

*** PROGRAM INSTRUCTIONS ***

This section will cover the libraries used for our experiments and code intructions that need to be followed to reproduce our results.

Libraries Used: numpy, pandas, matlibplot, seaborn, opencv, keras, scikit-learn, tensorflow.

** AdultData_Project **

All of the coding is done in Jupyter Labs and as such, the code is broken down into blocks (Heading blocks are excluded). 

Run a corresponding block to generate similar results in our experiment.

To run a block be sure to convert it from 'Raw NBConvert' format to 'Code' in the notebook.

block 7: To delete missing values that are represented by "?"
block 8: to keep missing values but encoding them, represented as 0
block 9: Removes 'United States' from the country column
block 14: Deletes column 'native_country'
block 16: This block lets you select the desired number of features e.g, X = dataset[:,0:6] only selects features.

** CIFARData_Project **

All of the coding is done in Jupyter Labs and as such, the code is broken down into blocks (Heading blocks are excluded). 

Run a corresponding block to generate similar results in our experiment.

To run a block be sure to convert it from 'Raw NBConvert' format to 'Code' in the notebook.

For GreyScale Images: Run block 10 and 11, however you will need to change the input_shape parameter for both LSTM and CNN models, which are mentioned in the code commnents. Also, disable block 24 (For LSTM) if using the greyscale setting.

For OneShot Encoding: To encode the labels, run block 14 and 15 but be sure to disable (convert to Raw NBConvert block) block 13. Also keep in mind to use appropiate loss function, which is mentioned in the comments.

To Normalize the data: activate/disable block 18.

*** RESULTS & CONCLUSION ***

In the experiments, we can observe key insights into how some of the models are functioning and performing based on different variations of data that we fed into them. 

First, ensemble models perform the best on average based on the classification and prediction of data, even if the dataset is missing values or has few features. 

Second, deep learning models also performed well, which is not surprising considering their nature. However, they are not always the ideal candidate models for your dataset as we have seen in our results; if the dataset is not overly huge in volume or complicated (like CIFAR), the traditional classification models will always perform better.

Third, different variations of data do impact the performance of the models, however, this is noticeable only for linear models and not for deep learning models, which are really difficult to interpret, we can point out which deep learning model performed better, but to what extent and how the classifications are calculated is still a mystery.

The hope is that such analysis will be helpful to future practitioners and students in the field as this study can be used by future researchers to analyze these models further with different parameters and datasets.