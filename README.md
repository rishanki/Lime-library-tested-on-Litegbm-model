Explaining Complex models like Litegbm using the LIME package.

The following notebook explores the famous lime library package which was published in
“Why Should I Trust You?” Explaining the Predictions of Any Classifier. By Marco Tulio Ribeiro, Sameer Singh and Carlos Guestrin from the University of Washington in Seattle(https://arxiv.org/pdf/1602.04938.pdf) . lime is able to explain all models for which we can obtain prediction probabilities. It makes use of the fact that linear models are easy to explain because they are based on linear relationships between features and class labels: The complex model function is approximated by locally fitting linear models to permutations of the original training set.

On each permutation, a linear model is being fit and weights are given so that incorrect classification of instances that are more similar to the original data are penalized (positive weights support a decision, negative weights contradict them). This will give an approximation of how much (and in which way) each feature contributed to a decision made by the model.
 
 Here we have built a model using the famous Litegbm classification package and tried explaining this complex model using LIME.
 
 Note: The telecom churn data can be found on- https://www.ibm.com/communities/analytics/watson-analytics-blog/predictive-insights-in-the-telco-customer-churn-data-set/
 
