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
![image](https://github.com/user-attachments/assets/10dfd5b4-30b9-4ed0-ac4e-e0849ac087ec)

## Stacking Ensemble Learning
Stacking has its own nomenclature where ensemble members are referred to as level-0 models and the model that is used to combine the predictions is referred to as a level-1 model.

The two-level hierarchy of models is the most common approach, although more layers of models can be used. 
For example, instead of a single level-1 model, we might have 3 or 5 level-1 models and a single level-2 model that combines the predictions of level-1 models in order to make a prediction.
### The key elements of stacking as follows:

Unchanged training dataset.   
Different machine learning algorithms for each ensemble member.  
Machine learning model to learn how to best combine predictions.  
