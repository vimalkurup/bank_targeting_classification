Link to Jupyter notebook: https://github.com/vimalkurup/bank_targeting_classification/blob/master/M17_Bank_Marketing_Application.ipynb
GitHub Repo: https://github.com/vimalkurup/bank_targeting_classification

Business Problem
Objective is to identify customers likely to subscribe to a term product offered by banks to it's customers by direct outbound reach

Recommendation
- Decision Tree and SVM models would identify maximum Sales conversion while Logistic regression and KNN is too conservative and doesn't serve the Business Purpose
- While Decision tree minimizes in-vain marketing pursuits, the model is more generalized with SVM; Hence recommendation is to use SVM Model for Marketing Campaign

Technicality
- Pandas for data reading/wranging/cleanup
- Seaborn for Visualization
- SKLearn for Pipelines, Encoding, CV, Stratification, Grid search

Models evaluated
- Logistic Regression
- SVM
- KNN
- Decision Trees

Assumptions
- Data sources state that a customer could be part of multiple campaigns; However, there is no customer identifier to seggregate Test and Training to ensure that model doesn't predict on the same customer that was trained on
  
Credits
- https://github.com/toby-gardner-ai/uc-berkeley-aiml-course/blob/main/notebooks/Mod4_Data_Analytics.ipynb
- For Unbalanced classes, papers suggest usage of AUPRC(Area under Precision-Recall curve) over F1- Macro Citation: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0118432

Limitations
- Limited images uploaded because of space constraint. 
- Randomized Grid Search performed on SVM instead of GridSearch due to latency constraints
