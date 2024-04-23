# Data &amp; Information Quality
## Dimentionality Reduction &amp; De-duplication to improve data quality

### Abstract

This is the final project for Data &amp; Information Quality course @Polimi. the goal of this project is to prepare the data for some Machine Learning tasks and increase the quality of data, not only the traditional aspects of data quality but also the new DQ issues.

### Project structure

The general pipeline used for this project is as follows:

<img width="1021" alt="image" src="https://github.com/salidotir/Data-Information-Quality/assets/35997721/a031eb1e-3949-49ae-a7cf-fa9158617fdb">

1. Data Collection
   - Create dataset with fixed default parameters
  
2. Data Pollution Function
   - Inject errors/values related to the assigned DQ issue at different (%)
  
3. Data Analysis and Evaluation
   - Metrics: Performance (F1 weighted score), Distance between train & test performances (F1 weighted score), Speed of training
  
4. Data Preparation
   - Apply different DQ improvements to correct the injected DQ issue
  
5. Data Analysis and Evaluation
   - Performed again after fixing the issues

6. Compare the obtained results


The chosen ML task here is classification and we decided fix two DQ issues, dimensionality and duplication.

- Duplication
  — 10 experiments with different % similarity: for example, creating and adding non-exact duplicated rows, based on a fixed similarity measure
  — For one experiment: varying % duplicated rows, for example from 5% to 50% (with an increasing step of 5%) of duplicated rows
- Dimensionality
  — 10 experiments with fixed number of samples and varying number of features
  — 10 experiments with fixed number of features and varying number of samples
