Name of Project:
Class Assignment 4-Ensemble Methods

Project Overview:
This project uses RandomForestClassifier, AdaBoostClassifier, GradientBoostClassifier, and XGBRFClassifier to train, test, and automate several ensemble method models and compare their performance based on Accuracy and AUC scores. 

Configuration/Installation Instructions:
To begin this project, you need to open a colab or Jupyter notebook and import the following packages: pandas, numpy, matplotlib.pyplot, sklearn preprocessing, sklearn.ensemble RandomForestClassifier, AdaBoostClassifier, and GradientBoostClassifier, amd sklearn metrics. Next, you need to uplad the Census Data.csv and read it in as a dataframe by using pd.read_csv('census_data.csv')

Files Included:
This assignment contains a README file, Written Responses PDF, and CA04-EnsembleMethods.ipynb

Known Bugs:
In Part 5, the error: cannot concatenate object type <class function>; must be Series or DataFrame is present. I am not sure why this is happening because, in the function  created for each Classifier, the results variable transforms the data into a Dataframe using pd.Dataframe('test_scores'). In an earlier version of the code I tried to use pd.Series('title_scores') instead to see is running them as pandas Series would work, but I still got the same error. Without this error, Part 5 should concatenate all the results frome each function into a DataFrame with the Index as 'Accuracy' and 'AUC' and the column headings as the Classifier names. 