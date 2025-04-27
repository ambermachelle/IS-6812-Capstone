# Predictive Modeling for Loan Default Prediction

## Business Problem Statement
Home Credit faces challenges in predicting loan defaults, leading to two major issues:
1. They lose business from applicants who could repay the loan but get rejected.
2. They approve applicants who end up defaulting, causing financial losses.

### Benefits of a Solution
By implementing a predictive modeling solution, Home Credit will be able to predict loan defaults with higher accuracy. This will allow them to maximize revenue by reducing the number of defaults.

## Project Details and Deliverables
The deliverable for this project is a predictive model that Home Credit can use to assess each new applicant’s likelihood of defaulting.

## STAR Analytics' Solution
Our team tested multiple models (logistic regression, decision trees, naive Bayes, etc.) but ultimately selected an XGBoost model. The XGBoost model outperformed all benchmark performance metrics set by the majority classifier. It was designed to be robust, scalable as Home Credit’s borrowing population grows, and easily integrable into their existing infrastructure to deliver real-time predictions when applications are submitted.

## My Contribution
During the modeling process, I was responsible for testing logistic regression models. I tested two models against the benchmark: a default model with no specifications and one with two interaction terms. Although both models performed decently in terms of accuracy, they failed to outperform the accuracy and AUC score set by the majority classifier, making them unfit for this competition.

In addition to model training, I assessed the feature importance of our best model (XGBoost) to extract meaningful insights from the model outputs. See the next section for more on those important predictors!

## Business Value
High-performing models are crucial for Home Credit because accurate predictions translate into reduced financial losses, better risk management, and increased trust from borrowers. Our model, once implemented, will help Home Credit make better application decisions and potentially expand its borrowing base.

Although the model is complex and not easily interpretable, it provides valuable insights into which predictors can help refine Home Credit’s loan criteria. For example, we found that older borrowers (retirement age) are less likely to default. Home Credit can use this insight to offer higher-value or more profitable products tailored to older borrowers with less risk. Similarly, we found that different income types (with varying levels of stability) show different likelihoods of default. With this insight, Home Credit can adjust loan offers based on income stability, minimizing risk while maximizing profitability.

## Difficulties
On the data side, the dataset was heavily imbalanced. The target variable (whether a borrower defaulted) was split about 92% to no default and 8% to default. Because of this imbalance, the majority classifier benchmark was very high at 92%, making it difficult to find a model that significantly outperformed it. In the end, our XGBoost model did outperform the majority classifier, but not by much!

On the people side, this was my first project involving group programming. One of the biggest challenges was creating a cohesive notebook that integrated everyone’s code. We went through multiple iterations to finally produce a functioning notebook. Although it was challenging to merge different coding styles, it was an incredibly valuable experience that taught me how to make my code more integrable and collaborative-friendly for future projects.

## What I Learned
The biggest takeaway from this project is that a high-performing model doesn’t mean much if you can't translate the results into business value. During the modeling process, we were heavily focused on finding the highest-performing model and didn’t think enough about interpreting the results. I now see that the real magic happens at the intersection of data and business — when an analyst can use highly technical methods to produce actionable, valuable insights that drive business decisions.

