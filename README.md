# XGBoost

XGBoosting (Extreme Gradient Boosting) is an extension of the Gradient Boosting method. It is one of the ensemble methods where a model is created through multiple iterations. 
Mainly there are two ensemble methods, viz; bagging and boosting. In Bagging we combine predictors from multiple-decision trees through a majority voting mechanism. In Boosting we build models sequentially by minimizing the error from previous models while increasing (or boosting) influence of high-performance models. It works in such a way that it calculates the error in first observation. This error is fed into the next model as input and new value is predicted. That error is again given as input to next model. This cycle continues until the ensemble of models is obtained. This is why it is called extreme gradient boosting.

In order to start the cycle, we make naïve predictions which are not accurate. This triggers the cycle and the process continues. The basic property of decision trees is utilized here. All the trees have same depth and can go for majority rule at each node.

The xgboost function has mainly 3 attributes; data, nround and objective. ‘nround’ refers to the number of iterations done and objective refers to the type of process. XGBoost follows the gradient descent algorithm where the iterations lead to a model with least (approximately zero) error. XGBoost is optimized GradientBoosting algorithm through parallel processing, tree-pruning,handling missing values and regularization to avoid overfitting/bias.   
