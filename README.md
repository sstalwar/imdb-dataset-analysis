# imdb-dataset-analysis

Problem 1: We need functions to assess and evaluate the
performance of our models. We will implement those first.
Create one function to calculate precision, one function to calculate recall and
one function to calculate f-measure.
Your function should look something like this: get_precision(y_pred, y_true)
Where y_pred is the set of predictions from your classifier and y_true is the set
of true (annotated/ground truth/gold) labels.
NOTE: Do not use sklearn built in functions to accomplish this – you are
supposed to write your own functions.
For this part of the assignment, you will be using the Large Movie Review
Dataset [1] – uploaded to Canvas in assignment 2 folder.
[1] Maas, A. L., Daly, R. E., Pham, P. T., Huang, D., Ng, A. Y., & Potts, C. (2011,
June). Learning word vectors for sentiment analysis. In Proceedings of the 49th
annual meeting of the association for computational linguistics: Human
language technologies-volume 1 (pp. 142-150). Association for Computational
Linguistics.
It contains movie reviews in two classes – positive and negative. The dataset is
split into training and test directories already. Raw text and already processed
bag of words formats have also been provided by the authors – c.f. README in
the directory.

Problem 2 : Majority Class Baseline. We will create majority class
baseline to evaluate our initial model performance – which is the simplest
baseline. The label for the test data should be the majority class found in
training data.
You should report P, R and F-score (using the functions you wrote to solve
Problem 1) for both training and test data to obtain full marks on this problem.

Problem 3: Review Length Baseline. We will create baseline to
evaluate our model performance – which takes into account length of the
review.
For this baseline, you should try setting various thresholds of review length to
classify them as positive or negative. For example, all reviews > 50 words in
length can be classified as positive. You should experiment with at least 3
different thresholds and document your reasons why you chose these
thresholds.
For each threshold, you should report P, R and F-score (using the functions you
wrote to solve Problem 1) for both training and test data to obtain full marks on
this problem.

Problem 4 : Implementing the Naïve Bayes classifier. You can use the
built-in Naive Bayes model from sklearn to train a classifier. Here is the
documentation for how to implement GaussianNB (discussed in class) using
sklearn.
You will train your classifier on the words contained in the positive and negative
reviews, based on the algorithm discussed in class.
You should report P, R and F-score (using the functions you wrote to solve
Problem 1) for both training and test data to obtain full marks on this problem.

Problem 5** : Implementing your own classifier. You can implement
your own classifier – by using another classifier from sklearn package – SVM or
Logistic Regression (for example) or you can experiment with different features
and add them to your Naïve Bayes model. As before, you should report P, R and
F-score (using the functions you wrote to solve Problem 1) for both training and
test data to obtain full marks on this problem.
