## Machine-learning
1. We take training data and develop our algorithms
1. Then we test the algorithm using our test data
1. We do it for other algorithms as well and then compare their results.
1. The goal is to find the algorithm that suits you (*fancy,newest,bestest algortihm doesn't mean it will suit your case*)
1. Confusion matrix is one great way to do that. It's out 2x2 matrix, where *rows are actual results* and *columns are predicted results*
######                *Yes*   *No*
###### (true positive)*178* *50*(false negative)
######                  -    -
###### (true negative) *50* *12*(true negative)
##### *178/178+50 = 0.78* - sensitivity
##### *12/12+50 = 0.19* - specificity

1. We can also calculate *sensitivity* and *specificity*
1. In the context of predicting how many people have a heart disease, *sensitivity* is how many people we predicted to have a heart disease
1. While *specificity* is how many people we predicted *not* to have a heart disease.
1. To calculate sensitivity - predicted result / predicted result + actual result, which will give the percent of correctness
1. Same with specificity, but for a different row/column
1. *If algorithms perform similarly* - 1st algorithm - 0.83 sensitivity, 0.85 specificity. 2nd algorithm - 0.81 sensitivity, 0.87 specificity
1. It varies on our needs. If we much rather our algorithm to have a higher accuracy on *true positives* (identifying people with heart disease), then we'd choose 1st algorithm
