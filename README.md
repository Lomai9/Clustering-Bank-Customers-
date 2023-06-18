# Clustering-Bank-Customers-

The data is a bank card transaction and user (card) loyalty analysis dataset
provided by a bank in Brazil. This assignment aims to practice on topics covered
in lectures 1-3, i.e., data quality analysis, statistical analysis, and regression
analysis given the dataset. The overall purpose of the analysis is to predict a
loyalty score for each card id represented in userscore.csv.
The dataset contains four files.
userscore.csv contain card ids and information about the card itself - the
first month the card was active. It also contains the predict/analysis target,
i.e., score, which is a score calculated by the bank, indicating the loyalty of
each card owner. Three features are provided, all of which are anonymized card
categorical features.
merchants.csv contains aggregate information for each merchant id represented in the data set. merchants can be joined with the transaction sets to
provide additional merchant-level information.
The historical transactions.csv and new merchant transactions.csv files contain information about each card’s transactions. historical transactions.csv contains up to 3 months’ worth of transactions for every card at any of the provided
merchant ids. new merchant transactions.csv contains the transactions at new
merchants (merchant ids that this particular card id has not yet visited) over
two months.
historical transactions.csv and new merchant transactions.csv are designed
to be joined with userscore.csv and merchants.csv. They contain information
about transactions for each card, as described above.
Given the dataset, answer the following questions. Your submission will be
judged based on your answer’s relevance and your regression model’s performance.

This assignment aims to practice unsupervised analysis, i.e., clustering and frequent
pattern mining.

3 Clustering Analysis
Q1 (30 points) Our goal is to cluster users based on their spending behaviors. Your task is to perform a clustering analysis leveraging the K-means
method and report your findings. You should specify how you select the
right ”K” for the k-means method, and how you create features. Explain
the resultant clusters (the meaning of each cluster) and judge the quality
of resultant clusters.
Q2 (5 points) Based on your results from Q1, report the statistics of loyalty
scores for each cluster of users. Report your findings.
Q3 (30 points) Discuss whether you need to reduce the dimensions to
improve clustering performance and build another clustering model (if
you believe dimension reduction would help, you can apply it or choose
another clustering method) to improve your analysis from Q1. You should
explain why the resultant clusters are better than the ones you got in Q1.
Q4 (5 points) Based on your results from Q3 report the statistics of loyalty
scores for each cluster of users. Report your findings.
4 Frequent Pattern Mining
You can consider the mlxtend library1 or the spmf library2
Q5 (20 points) Use frequent pattern mining to find frequently co-occurring
transaction types. Report your findings and justify how you pick the min
support threshold.
Q6 (10 Points) Redo Q5 by splitting users based on their loyalty scores.
The goal is to explore if different frequent patterns exist in users with
high/low loyalty scores.
