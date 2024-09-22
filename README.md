# EnsembleTechniques
Ensemble learning refers to algorithms that combine the predictions from two or more models.
The three main classes of ensemble learning methods are bagging, stacking, and boosting.

## Bagging Ensemble Learning
The name Bagging came from the abbreviation of Bootstrap AGGregatING. As the name implies, the two key ingredients of Bagging are bootstrap and aggregation.
This typically involves using a single machine learning algorithm, almost always an unpruned decision tree, and training each model on a different sample of the same training dataset. 
The predictions made by the ensemble members are then combined using simple statistics, such as voting or averaging.   
### The key elements of bagging as follows:
Bootstrap samples of the training dataset.  
Unpruned decision trees fit on each sample.  
Simple voting or averaging of predictions.  
