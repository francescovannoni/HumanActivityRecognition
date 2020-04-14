# HumanActivityRecognition
This project aims to build a decision tree that predicts the human activities such as Walking, Walking Upstairs, Walking Downstairs, Sitting, Standing and Laying from the Sensor data of smart phones.

## Repository Overview:
The repository has 5 ipython notebook  
- data pre-processing.ipynb : import datas, check for null and duplicated and show graphs (using matplotlib, TSNE and seaborn)  
- visualization.ipynb : show a subtree (using sklearn.export_graphviz)    
- ccp_alpha analysis.ipynb : check for appropriate values of ccp_alpha, train decision tree, compare performance   
- ccp_alpha res: generate confusion matrix and classification report using results of ccp_alpha analysis  
- cross validation: use GridSearchCV for hyperparameter tuning and generate confusion matrix using best estimators

## Dataset:
The dataset can be downloaded from ->
https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones#  

To reuse the code you only need to change the path in pandas.read_csv(...) used to import datas

## Requirements:
All the code is written in python 3

### Dependencies
- numpy
- pandas
- matplotlib
- seaborn
- sklearn
- itertools
- pydotplus
- mpl_toolkits

## References:
Part of the code for ccp_alpha analysis comes from ->    
https://scikit-learn.org/stable/auto_examples/tree/plot_cost_complexity_pruning.html 

To make a pretty plot of the confusion matrix ->  
https://github.com/DTrimarchi10/confusion_matrix  
