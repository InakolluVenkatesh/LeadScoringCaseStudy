# Lead Scoring Case Study Summary

## Problem Statement

X Education sells online courses to industry professionals and needs help in selecting the most promising leads, i.e., the leads that are most likely to convert into paying customers. The company requires a lead scoring model that assigns a lead score to each lead, where leads with higher scores have a higher conversion chance.

The CEO has set a target lead conversion rate of approximately 80%.

## Solution Summary

### Step 1: Reading and Understanding Data

- Read and analyze the data.

### Step 2: Data Cleaning

- Drop variables with a high percentage of NULL values.
- Impute missing values with repeated values for categorical variables.
- Create new classification variables for categorical variables.
- Identify and remove outliers.

### Step 3: Data Analysis

- Perform Exploratory Data Analysis (EDA) to understand the data.
- Remove irrelevant variables for model training.

### Step 4: Creating Dummy Variables

- Create dummy variables for categorical variables.

### Step 5: Test-Train Split

- Divide the dataset into training and testing sets with a 70:30 proportion.

### Step 6: Feature Rescaling

- Apply Min-Max scaling to rescale the original numerical variables.
- Create an initial model using the stats model to obtain statistical insights.

### Step 7: Feature Selection using RFE

- Use Recursive Feature Elimination (RFE) to select the top 20 important features.
- Recursively analyze model parameters to select significant variables and drop insignificant ones.
- Identify 15 significant variables with acceptable VIF values.

### Step 8: Plotting the ROC Curve

- Plot the ROC curve for the selected features.
- Achieve an area coverage of 88%, indicating the model's reliability.

### Step 9: Finding the Optimal Cutoff Point

- Plot probability graphs for Accuracy, Sensitivity, and Specificity.
- Determine the optimal cutoff point at the intersection of these graphs.
- Find the cutoff value to be 0.36.
- Observe approximately 80% correctly predicted values based on the new cutoff.
- Calculate accuracy (80%), sensitivity (83%), and specificity (79%) values.

### Step 10: Computing Precision and Recall Metrics

- Calculate precision (71%) and recall (82%) metrics on the train dataset.

### Step 11: Making Predictions on Test Set

- Implement the learnings on the test dataset.
- Calculate conversion probabilities based on Sensitivity and Specificity metrics.
- Obtain accuracy (80%), sensitivity (80%), and specificity (79%) on the test set.

This summary provides an overview of the lead scoring case study, outlining the steps followed and the key findings and metrics obtained throughout the process.
