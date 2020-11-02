![NBA_logo](https://seeklogo.com/images/N/nba-logo-41668C66DB-seeklogo.com.png)

# NBA Playoff Modelling 
This notebook aims to predict a NBA teams probability of making the playoffs based on their team stats. 

Additionally, the notebook contains a full exploratory data analysis that covers the characteristics of the dataset and the entire modelling process from preprocessing, feature engineering, and training. 

The raw data can be found on [Basketball Reference](https://www.basketball-reference.com/) and the tabular data can be found on my [Kaggle](https://www.kaggle.com/jpsdev/19802019-nba-team-stats)

# Model Summary 
3 models were all trained on a 80/20 - test/validation set. The additional features were calculated from the initial data collected from Basketball Reference. More information of how the additional features were calculated [here](https://www.nbastuffer.com/analytics-101/)

Pipelines were created for the logistic, and support vector machine (SVM) models - where features were standardized. 

## Modelling Metrics
|                                              |           |            |           |           |
|----------------------------------------------|-----------|------------|-----------|-----------|
| Model                                        | Precision | Recall     | F1 Score  | Accuracy  |
| \*Baseline\* Logistic Classifier             | 0\.858333 | 0\.851240  | 0\.854772 | 0\.841629 |
| \*Optimized\* Logistic Classifier            | 0\.850000 | 0\.842975	 | 0\.846473 | 0\.832579 |
| \*Baseline\* Random Forest Classifier        | 0\.830645 | 0\.851240  | 0\.840816 | 0\.823529 |
| \*Optimized\* Random Forest Classifier       | 0\.833333 | 0\.867769  | 0\.850202 | 0\.832579 |
| \*Baseline\* Support Vector Machine \(SVM\)  | 0\.878049 | 0\.892562  | 0\.885246 | 0\.873303 |
| \*Optimized\* Support Vector Machine \(SVM\) | 0\.861789 | 0\.876033  | 0\.868852 | 0\.855204 |

- The optimized models were optimized based on the **precision**, but only the Random Forest benefitted from the optimization. 

# Technologies Used
## Modelling
- [Scikit-learn](https://scikit-learn.org/stable/)
## Analysis
- [Numpy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
## Visuals/Graphs
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)

---
Note: not directly associated with the NBA or Basketball Reference