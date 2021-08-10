# Apply-Naive-Bayes-on-Donors-Choose-dataset

### Assignment: Apply NB on Donors Choose dataset.<br/>
1. Apply Multinomial NB on these feature sets<br/>
Set 1: categorical, numerical features + preprocessed_eassay (BOW)<br/>
Set 2: categorical, numerical features + preprocessed_eassay (TFIDF)<br/>

2. The hyper paramter tuning(find best alpha:smoothing parameter)<br/>
- Find the best hyper parameter which will give the maximum AUC value
- find the best hyper paramter using k-fold cross validation(use GridsearchCV or RandomsearchCV)/simple cross validation data (write for loop to iterate over hyper parameter values)

3. Representation of results<br/>
- You need to plot the performance of model both on train data and cross validation data for each hyper parameter.<br/>
- Once after you found the best hyper parameter, you need to train your model with it, and find the AUC on test data and plot the ROC curve on both train and test.
- Along with plotting ROC curve, you need to print the confusion matrix with predicted and original labels of test data points.

4. Fine the top 20 features from either from feature Set 1 or feature Set 2 using absolute values of `feature_log_prob_ ` parameter of `MultinomialNB` (https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html) and print their corresponding feature names

5. You need to summarize the results at the end of the notebook, summarize it in the table format
