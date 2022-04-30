# OVERVIEW
The purpose of this analysis was to determine whether any of the algorithms we created are suitable for commercial use in predicting whether or not to approve a loan for an individual. We used speicific criteria to feed into the algorithm to determine this. 

## RESULTS
- Naive oversampling resulted in a precision score of 0.01 and recall of 0.62. The F1 score of 0.02 reflected athe low precision score
-  SMOTE oversampling similarly resulted in a precision score of 0.01 and recall of 0.61, and a F1 score of 0.02.
-  A model with undersampling yielded similarly poor results, with a precision score of 0.01, recall of 0.65, and F1 score of 0.01.
-  Combination sampling resulted in a precision score of 0.01 and recall of 0.70, and a F1 score of 0.02. Even though this model did better than other models, it was still performing under expectations
-  The balanced random forest classifier's precision is 0.04, meaning that in 100 loan applications that were flagged to be bad, only 4 were actually bad loan applications. The model's recall/sensitivity is 0.67, meaning that it detected 67% of bad loan applications. The F1 score is low at 0.07, since either a low precision or recall will result in a lower F1 score.
-  The random forest classifier with AdaBoost, while achieving better results, still suffered from inadequate predictive power. Its precision score is 0.09 and its recall 0.92. The F1 score, again, is skewed low at 0.16 by the low precision score

## SUMMARY
Overall, none of the sampling methods returned usable results. The accuracy of each of them would not bode well for any type of commercial use and would end up causing more issues than solving. 
