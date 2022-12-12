# Pipelines and Grids:
## a machine learning practice project in Python working with Scikit-Learn pipelines and grid search. 
<br/>
The dataset I am working with records permissions for Android apps and their status as malware or benevolent. It can be found at https://archive-beta.ics.uci.edu/api/static/ml/datasets/722/data.csv and was collected to be the basis of a paper on malware classification (Mathur, Akshay, et al. "NATICUSdroid: A malware detection framework for Android using native and custom permissions." Journal of Information Security and Applications 58 (2021): 102696.) The dataset is, unsurprisingly, very well suited and prepared for comparing the performance of different classification models, since that is part of what Akshay et. al. are doing as well. 

Here this is only implemented on a toy scale of course, most importantly, I have tried to keep the runtime of this notebook in check, since grid searches can take a lot of time, especially with sophisticated models, promising candidates are often not included (e.g. GBMs).

The plan is to compare pipelines with three different kinds of model, K Nearest Neighbors, Logistic Regression and Random Forest, with scaling and feature selection as data preprocessing steps. The best parameters for each pipeline will be found through grid search and then the three winners will compete on the test data.
