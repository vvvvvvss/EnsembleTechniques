# Ensemble Techniques
Ensemble methods is a machine learning technique that combines several base models in order to produce one optimal predictive model.
It can be used for classification and regression.
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
![image](https://github.com/user-attachments/assets/d9b3c7ce-4c7d-4beb-891d-713ae6a87147)

## Boosting Ensemble Learning
Boosting is an ensemble method that seeks to change the training data to focus attention on examples that previous fit models on the training dataset have gotten wrong.
This typically involves the use of very simple decision trees that only make a single or a few decisions, referred to in boosting as weak learners. 
The predictions of the weak learners are combined using simple voting or averaging, although the contributions are weighed proportional to their performance or capability. 
The objective is to develop a so-called “strong-learner” from many purpose-built “weak-learners.”
### The key elements of boosting as follows:

Bias training data toward those examples that are hard to predict.   
Iteratively add ensemble members to correct predictions of prior models.  
Combine predictions using a weighted average of models.  
![image](https://github.com/user-attachments/assets/bc6d1495-c37e-4e4d-92ca-79b53642a84b)  
![image](https://github.com/user-attachments/assets/57e4e9b4-7703-45e8-bfda-b5cd8ad21071)


## Conclusion

**Bagging** involves fitting ***many decision trees*** on different samples of the _same dataset_ and averaging the predictions.  
**Stacking** involves fitting ***many different models*** types on the _same data_ and using another model to learn how to best combine the predictions.  
**Boosting** involves adding ***ensemble members*** sequentially that _correct the predictions_ made by prior models and outputs a weighted average of the predictions.  



#### Other references
https://www.analyticsvidhya.com/blog/2018/06/comprehensive-guide-for-ensemble-models/
