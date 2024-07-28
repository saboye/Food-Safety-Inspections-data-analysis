<div align="center">
  <h1> Enhancing Food Safety Inspections in Chicago Through Data Mining</h1>
</div>

<p align="center">
    <img src="https://img.shields.io/github/contributors/saboye/Analyzing-Crime-Trends-in-Omaha?color=blue&logo=github&style=for-the-badge" alt="GitHub contributors" />
    <img src="https://img.shields.io/github/forks/saboye/Analyzing-Crime-Trends-in-Omaha?logo=github&style=for-the-badge" alt="GitHub forks" />
    <img src="https://img.shields.io/github/issues-raw/saboye/Analyzing-Crime-Trends-in-Omaha?style=for-the-badge" alt="GitHub issues" />
    <img src="https://img.shields.io/github/license/saboye/Analyzing-Crime-Trends-in-Omaha?style=for-the-badge" alt="GitHub license" />
    <img src="https://img.shields.io/github/last-commit/saboye/Analyzing-Crime-Trends-in-Omaha?style=for-the-badge" alt="GitHub last commit" />
    <img src="https://img.shields.io/badge/pandas-1.3.5-blue?style=for-the-badge&logo=pandas" alt="Pandas" />
    <img src="https://img.shields.io/badge/numpy-1.20.3-blue?style=for-the-badge&logo=numpy" alt="NumPy" />
    <img src="https://img.shields.io/badge/scikit--learn-0.24.2-blue?style=for-the-badge&logo=scikit-learn" alt="scikit-learn" />
    <img src="https://img.shields.io/badge/matplotlib-3.4.2-blue?style=for-the-badge&logo=matplotlib" alt="Matplotlib" />
</p>

## Overview

This repository contains an analysis of food safety inspections in Chicago, aiming to enhance public health through data mining techniques. The project identifies patterns in inspection data, develops predictive models, and provides actionable insights to prioritize high-risk establishments.

## Contents

- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Importance and Utility](#importance-and-utility)
- [Stakeholder Engagement](#stakeholder-engagement)
- [Data Source](#data-source)
- [Field Name and Description](#field-name-and-description)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preparation](#data-preparation)
- [Modeling](#modeling)
- [Summary](#summary)
- [Conclusion](#conclusion)
- [Recommendations](#recommendations)
- [References](#references)

## Introduction

This project explores public health and safety through food establishment inspections in Chicago. By analyzing inspection data and applying predictive models, the goal is to proactively identify potential health code violations and enhance the efficacy of inspections.

## Problem Statement

Foodborne illnesses pose significant threats to public health and can severely impact the economy of affected businesses. This project aims to create a predictive system that can accurately forecast health code violations, allowing for prioritized inspections.

## Importance and Utility

A predictive system will improve inspection efficacy, enabling regulatory authorities to prioritize high-risk establishments and allocate resources effectively.

## Stakeholder Engagement

The project envisions a system where health inspectors can prioritize inspections based on predicted risks, leading to more efficient resource use and safer food for the public.

## Data Source

The dataset comprises records from the City of Chicago's official data portal, specifically from the Food Inspections dataset, including inspection dates, outcomes, types of violations, and geographic coordinates.

## Field Name and Description

- **Inspection ID**: Unique identifier for the inspection.
- **AKA Name**: Also Known As name of the facility.
- **License #**: License number of the facility.
- **Facility Type**: Type of facility (e.g., restaurant, grocery store).
- **Risk**: Risk category of the health inspection.
- **Address, City, State, Zip**: Location details.
- **Inspection Date**: Date when the inspection took place.
- **Inspection Type**: Type of inspection (e.g., Complaint, Canvass).
- **Results**: Outcome of the inspection (e.g., Pass, Fail).
- **Violations**: Descriptions of any violations found during the inspection.
- **Latitude, Longitude, Location**: Geographical coordinates.

## Exploratory Data Analysis (EDA)

EDA involves investigating and visualizing the dataset to uncover underlying patterns and relationships. Key analyses include:
- **Distribution of Inspection Results**: Frequency of various inspection outcomes.
- **Top 10 Facility Types by Number of Inspections**: Identifying the most frequently inspected establishments.
- **Risk Category Distribution**: Proportion of establishments by risk level.
- **Number of Inspections Over Time (Monthly)**: Temporal trends in inspection activities.
- **Map of Inspections**: Geographic distribution of inspections.

## Data Preparation

Effective data preparation steps include:
- **Dropping Unnecessary Columns**: Removing non-essential columns.
- **Handling Missing Values**: Filling missing values appropriately.
- **Transforming and Encoding Features**: Creating new features and encoding categorical variables.
- **Defining Target Variable and Features**: Setting the target variable and features for modeling.
- **Scaling Features**: Normalizing feature values.
- **Splitting the Data**: Dividing the data into training and testing sets.

## Modeling

The project uses logistic regression, decision tree, and random forest models to predict inspection outcomes. SMOTE is applied to balance the dataset, improving model performance. Key metrics include accuracy, precision, recall, and F1-score.

## Summary

Balancing the dataset using SMOTE significantly improved the models' ability to detect failed inspections. The Decision Tree and Random Forest models achieved a better balance between precision and recall, making them more suitable for identifying violations in food establishments.

## Conclusion

The analysis provided valuable insights into predicting food safety inspection outcomes. The Decision Tree and Random Forest models showed promise for practical use, though further validation and fine-tuning are necessary for deployment.

## Recommendations

1. **Model Selection**: Prioritize Decision Tree and Random Forest models for deployment.
2. **Ongoing Monitoring**: Implement continuous monitoring and evaluation.
3. **Feature Enhancement**: Explore additional variables and refine existing features.
4. **Hyperparameter Tuning**: Optimize model performance through hyperparameter tuning.
5. **Ensemble Methods**: Combine multiple models to improve prediction accuracy.

## References

- [City of Chicago Food Inspections Dataset](https://data.cityofchicago.org/)

