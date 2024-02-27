# Instacart-Market-Basket-Analysis
## Project Description
This study focuses on predicting customers next orders using a large dataset
released by Instacart on Kaggle. The dataset includes over 3 million orders from
more than 200,000 users. Advanced machine learning techniques such as XGBoost,
Light Gradient Boosting, and Logistic Regression are used in this project.
For detail information and data sets, here is the link (https://www.kaggle.com/competitions/instacart-market-basket-analysis)

### Data sets 

In this project, we have six data files: Department, Aisles, Products,
Orders, Order Products Prior, and Order Products Train. Each dataset provides
valuable insights into different aspects of the e-commerce platform. Let&#39;s take a
closer look at each dataset and its contents.

### Exploratory Data Analysis:
In the initial phase of the exploratory data analysis process, we started by
examining the summary information of our available datasets. By looking at the
distributions of classes within these datasets, we gained insights into their
characteristics. For instance, analyzing the percentage distribution of the eval set
column in the orders dataset provided a foundational understanding of its structure.
One notable observation across all datasets was the presence of a single NA
value, which we decided to remove for the integrity of our analysis.
** you can reach the details of eda process from Notebooks folder.

### Solution Approach

### Feature Engineering
In the field of retail analytics, particularly when working with datasets such
as Instacarts, the phase of feature engineering is of crucial importance. Feature
engineering can be broadly categorized into three segments: user-based features,
product-based features, and user-product features. This process heavily relies on the
group-by functionality provided by the pandas library, in addition to basic
mathematical operations performed on each column. In this discussion, we will focus
on the development and significance of user-based features.

* user-based features
* product-based features
* user-product-based features

** you can reach the details of feature engineering process from Notebooks folder.

To address the imbalance in the dataset, the 'stratify' parameter was used while splitting the dataset. Additionally, we experimented with oversampling techniques during the model development phase. However, as oversampling did not lead to significant improvements in model performance, it was not adopted in the final models.


### Modelling Approach

| MODELS         | Train F1 Score | Validation F1 Score | Private F1 Score | Public F1 Score |
|----------------|----------------|---------------------|------------------|-----------------|
| Random Forest  | 0.426          | 0.421               | 0.367            | 0.368           |
| Light GBM      | 0.445          | 0.436               | 0.364            | 0.366           |
| XG Boost       | 0.443          | 0.435               | 0.377            | 0.377           |
| Decision Trees | 0.417          | 0.416               | 0.364            | 0.366           |

** you can reach the details of feature engineering process from Notebooks folder.


## Results

The consistency across training, validation, and test scores suggests the absence of overfitting or underfitting in our models. This reliability across different data segments reinforced the robustness of our modeling approach.

Ultimately, based on the comprehensive evaluation of performance metrics, the XG Boost algorithm was selected as the most effective model. This model demonstrated superior accuracy in predicting future purchasing preferences of Instacart users.

** too reach whole project, please visit my profile.
