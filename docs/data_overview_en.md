## Business Context
  **What problem does the dataset aim to solve?**
 To understand the factors associated with candidates’ intention to change jobs.
**What decision could be made using these data?** 
The results can support decisions related to retention strategies, optimization of recruitment processes, and planning of training programs.
**What metric is critical?** 
target= intentio to change jobs (0/1).
## Dataset Structure
**What does a row represent?** A candidate.
**What does a column represent?** Candidate characteristics.
**What is the level of granularity?** Candidate-level granularity, where each row corresponds to a candidate and their associated attributes.
## Data Quality
** Are there missing values?** There are missing values in the following columns:
Missing Values Summary

| Column             | Missing Rows | Percentage |
|--------------------|--------------|------------|
| gender             | 4,508        | 23.53%     |
| enrolled_university| 386          | 2.01%      |
| education_level    | 460          | 2.40%      |
| major_discipline   | 2,813        | 14.68%     |
| experience         | 65           | 0.34%      |
| company_size       | 5,938        | 30.99%     |
| company_type       | 6,140        | 32.04%     |
| last_new_job       | 423          | 2.21%      |

**Are there duplicates?** The table does not show duplicated records.
**Are there out-of-range values?** The company_size column contains non-standardized values such as “10/49,” which require normalization for analysis.
**Are data types correct?** Data types are consistent with the content of each column; however, some variables representing numerical or ordinal values are stored as text and will require transformation during the data cleaning stage.
**Are there columns that will not be used?** The enrolled_id column corresponds to a technical identifier and does not add analytical value, so it could be excluded in later stages.
## Limitations and Assumptions
**What do these data NOT measure?** The dataset does not measure whether a job change occurred, only the intention to change, nor does it include job performance metrics.
**Are there biases?** The dataset is focused on data scientist profiles, which may introduce population bias and limits generalization to other job roles.
**Is key information missing?** The dataset does not include direct metrics related to organizational climate, corporate culture, or job satisfaction.
## Project Scope
This project focuses on descriptive and diagnostic analysis to identify factors associated with candidates’ intention to change jobs. Detailed activities, deliverables, and timelines are defined separately in the Scope of Work document. No predictive models are developed.
