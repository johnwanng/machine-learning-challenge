# machine-learning-challenge
Machine Learning Homework - Exoplanet Exploration

model_1.ipynb uses the support-vector machine model and its model's result is saved in the svm.sav file. This model only uses the following 5 columns as x values:
1. koi_fpflag_nt
2. koi_period
3. koi_time0bk
4. koi_impact
5. koi_duration. 

I have also chosen the following feature outcomes:

1. CONFIRMED
2. FALSE POSITIVE
3. CANDIDATE


Training and testing scores are 0.4 and 0.42 respectively.
Hyperparameter tuning has improved the result to 0.58 but I still think SVM might not be the model for this exercise as I think because of the number of feature outcomes. It would be more suited if there were only two features, e.g. TRUE or FALSE.


 
model_2.ipynb uses the k-nearest neighbors algorithm and its model's result is saved in the knn.sav file. It uses the same 5 columns as x values as well as the same 3 feature outcomes as the svm model above. The best k value is 7 and test accuracy is 0.633 which is better than the svm model above.

In summary, I think the most suitable model for this exercise should be the Random Forrest as such model is best fitted for multiple feature outcomes having more than two values like our example. As both SVM (more so with SVM) and KNN models suffered when feature outcomes contain more than 2 values.   



