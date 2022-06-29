# DataMining

The Boolean satisfiability (SAT) problem consists in determining whether a Boolean formula F is satisfiable or not. F is represented by a pair (X, C), where X is a set of Boolean variables and C is a set of clauses in Conjunctive Normal Form (CNF). Each clause is a disjunction of literals (a variable or its negation). This problem is one of the most widely studied combinatorial problems in computer science. It is the classic NP-complete problem. Over the past number of decades, a significant amount of research work has focused on solving SAT problems with both complete and incomplete solvers. Recent advances in supervised learning have provided powerful techniques for classifying problems. In this project, we see the SAT problem as a classification problem. Given a Boolean formula (represented by a vector of features), we are asked to predict if it is satisfiable or not. In this project, we represent SAT problems with a vector of 327 features with general information about the problem, e.g., number of variables, number of clauses, fraction of horn clauses in the problem, etc. There is no need to understand the features to be able to complete the assignment. The dataset is available at: https://github.com/andvise/DataAnalyticsDatasets/blob/main/dm_assignment2/sat_dataset_train.csv

This is original, unpublished data. The CSV file contains 1929 rows and 328 columns. The
first 327 columns contain the features. The last column (‘target’) contains the label; 0 for
unsatisfiable and 1 for satisfiable.


I started with KNN and decision tree and checked the accuracy of the models, after then I moved to tune my hyperparameters and did feature reduction. Lastly opt Random forest model using pipeline and created a single code cell that loads it and
evaluate it on the following test dataset: https://github.com/andvise/DataAnalyticsDatasets/blob/main/dm_assignment2/sat_dataset_test.csv


The accuracy was 99% of my model on Test data. For more info, please check the code.
