# Wontfix Issue Classification in Open-Source Software

## Overview

In software development, the term **"wontfix"** refers to issues that are identified but intentionally left unresolved due to low priority, perceived infeasibility, or other reasons. Efficiently detecting these **wontfix** issues is crucial for optimal resource allocation and backlog management.

Previous research on this topic has been limited, particularly in the context of large datasets. This study extends existing research by analyzing a significantly larger dataset, encompassing issues from top programming languages such as **JavaScript**, **Python**, **Java**, **TypeScript**, and **C#**.

## Data Collection and Analysis

We utilized GitHub’s **REST API** to collect data from **1,000 repositories**, filtering for quality and relevance. Ultimately, we analyzed **420 issue reports** from **200 projects** to identify the reasons behind the **wontfix** classifications.

### Key Findings:

- We uncovered **43 distinct reasons** for the **wontfix** classification, with **24 of these being newly identified**.
- Our **qualitative analysis** provided valuable insights into the patterns and causes behind wontfix issues.

## Quantitative Analysis

Following the qualitative analysis, we conducted a **quantitative analysis** to distinguish between **wontfix** and **non-wontfix** issues. Key findings include:

- Reporters with a smaller number of previously submitted issue reports are more likely to submit wontfix issue reports.

### Machine Learning Approach

To improve the detection of **wontfix** issues, we employed machine learning techniques, utilizing a large, imbalanced dataset with **43 features** categorized into the following areas:

- **Reporter experience**
- **Text dimensions**
- **Collaboration network**
- **Readability**
- **Completeness**

### Algorithm Selection

We used several machine learning algorithms to classify **wontfix** and **non-wontfix** issue reports, including:

- **J48**
- **Random Forest**
- **XGBoost**
- **Gradient Boosting**
- **Ensemble learning algorithms**

### Threshold Adjustment

We adjusted the threshold values for classification from **0.1 to 0.7** to observe variations in **accuracy** and **recall**. The results showed:

- Increasing the threshold improved **precision** but decreased **recall**, allowing developers to tune the threshold values based on their specific needs.

## Conclusion

The study highlights the complexity and multifaceted nature of **wontfix** issue classification. The insights gained from this research can improve issue management processes in software development, allowing teams to better allocate resources and handle backlogs effectively.

## Index Terms

- **Open-source software (OSS)**
- **Help wanted issues**
- **OSS project collaboration**
