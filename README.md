## Decision Tree and COnfusion matrix
# decision_tree
#confusion matrix
Confused about the prediction of the performance of your models, try a confusion matrix!

Not so funny, I guess.

 Each entry in the confusion matrix corresponds to the number of predictions made by the model where it classified the sample correct or incorrect. The confusion matrix also helps us to visualize the performance of different models and by comparing these models we can proceed with the one that has the highest accuracy.
 
Here the rows represent the instances of the class that has been predicted (by the algorithm that we used) and the columns represents the instances on the known true values. The values here represent for type of values inside the confusion matrix:

·       True Positive: They occur when we make a prediction and the observation actually belongs to the class that we had predicted.

·       True negatives: they occur when we predict that the observation did not belong to the class and the record did not belong there.

·       False positives: They occur when we predict that the observation belongs to the class whereby it did not. This type of error is called type-1 error.

·       False negative: this occur when we predict the record to not belong to the class whereby it really did. This type of error is called type-2 error and is more serious than type-1.



Terminology related to the confusion matrix:

·       Accuracy: The accurate values of the matrix are the true positives (TP) and the true negatives (TN), so the accuracy will be as follows:

              (TP+TN)/(TP+TN+FP+FN)

·       Precision: The fraction of predictions as a positive class that were truly positive.

(TP)/(TP+FP)

·       Recall: It stands for the fraction of all the positive samples that were correctly predicted as positive by the algorithm.

(TP)/(TP+FN)

·       F1-score: This combines the above stated parameters of precision and recall into one by taking their harmonic mean.

By looking at the above parameters we can safely say that ideally, we need a model that has a accuracy of one and the f1 score of 1. But that is rarely the case, so we compare our models using the confusion matrix based on the parameters mentioned above and use the one that has the best values.

Note, that the values stated above must not be treated as a standalone value to make any decisions, rather they must be used in congruence with each other to select a model. It must be kept in mind that these independent values are sensitive to the values contained in the dataset and if there is an imbalance in the number of entries of a single type the further values obtained will be inaccurate.

