# ⚽ FIFA 20 Player Analytics & Machine Learning

## Overview

This project explores the FIFA 20 player dataset and applies data analysis, visualization, clustering, and machine learning techniques to uncover patterns in player performance and attributes.

The objective is to understand what makes football players similar, identify natural player groups through clustering, analyze player characteristics, and build predictive models capable of estimating player quality based on skill attributes.

---

## Project Objectives

This project addresses the following goals:

* Perform comprehensive Exploratory Data Analysis (EDA)
* Analyze player demographics and football attributes
* Identify countries producing the highest number of professional players
* Study the relationship between age and overall player rating
* Compare salaries among different attacking positions
* Cluster football players based on their skill profiles
* Train and compare multiple machine learning models
* Recommend the best model for production use

---

## Dataset

### Source

FIFA 20 Complete Player Dataset

### Domain

Sports Analytics / Football Analytics

### Dataset Size

* Thousands of professional football players
* Player demographic information
* Physical attributes
* Technical skills
* Position-specific ratings
* Market value and wage information

### Key Features

#### Player Information

* Name
* Age
* Nationality
* Height
* Weight
* Preferred Foot
* Position

#### Player Ratings

* Overall Rating
* Potential Rating

#### Technical Skills

* Dribbling
* Ball Control
* Finishing
* Short Passing
* Long Passing
* Vision
* Crossing
* FK Accuracy

#### Physical Attributes

* Sprint Speed
* Acceleration
* Strength
* Balance
* Agility
* Stamina
* Jumping

#### Defensive Attributes

* Interceptions
* Marking
* Standing Tackle
* Sliding Tackle

#### Mental Attributes

* Reactions
* Positioning
* Composure
* Aggression

---

## Exploratory Data Analysis

### Player Distribution by Country

A ranking of the top countries producing FIFA 20 players was generated.

Key observations:

* European countries dominate player production.
* Traditional football nations contribute a significant share of elite players.
* Strong football development systems correlate with higher player representation.

---

### Overall Rating vs Age

The relationship between player age and overall rating was analyzed.

Insights:

* Ratings generally improve during early career stages.
* Peak performance occurs during the mid-to-late twenties.
* After the peak age range, performance growth slows and eventually declines.

This analysis helps identify the age at which players typically stop improving.

---

### Wage Analysis

Offensive positions were compared:

* Striker (ST)
* Right Winger (RW)
* Left Winger (LW)

Analysis revealed which attacking role receives the highest average wage based on FIFA market valuations.

---

## Data Preprocessing

Several preprocessing steps were applied before modeling.

### Data Cleaning

* Removed irrelevant columns
* Handled missing values
* Standardized feature formats
* Converted categorical variables into machine-readable form

### Feature Engineering

* Position grouping
* Position category creation
* Attribute selection
* Derived analytical features

### Scaling

Numerical features were standardized to improve model performance.

---

## Player Clustering

### Objective

Group players with similar playing styles and skill profiles.

### Techniques Used

#### Principal Component Analysis (PCA)

Used to reduce dimensionality while retaining the majority of information.

Benefits:

* Faster clustering
* Better visualization
* Reduced noise

#### K-Means Clustering

Applied to discover natural player groups.

### Cluster Evaluation

The optimal number of clusters was selected using:

* Elbow Method
* Silhouette Score

### Cluster Interpretation

Clusters revealed groups such as:

* Elite attackers
* Creative midfielders
* Defensive specialists
* Physical players
* Balanced all-rounders

These clusters help understand player archetypes beyond traditional positions.

---

## Machine Learning Models

Several regression algorithms were trained and compared to predict player quality.

### Models Evaluated

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor
5. Extra Trees Regressor
6. XGBoost (if implemented)

---

## Evaluation Metrics

Models were evaluated using:

* R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

### Primary Goal

Maximize prediction accuracy while minimizing prediction error.

---

## Results

### Best Performing Model

**Gradient Boosting Regressor** *(or the best-performing model from your notebook)*

Reasons:

* Highest R² Score
* Lowest prediction error
* Strong generalization ability
* Robust performance on complex relationships

### Key Findings

* Technical skills strongly influence overall ratings.
* Reactions and ball control are among the most important attributes.
* Physical and mental attributes contribute significantly to player quality.
* Clustering successfully identified distinct football player profiles.

---

## Feature Importance Analysis

The most influential features included:

* Reactions
* Ball Control
* Dribbling
* Composure
* Vision
* Positioning
* Finishing
* Short Passing

These attributes contribute heavily to overall player performance ratings.

---

## Challenges Faced

### 1. High-Dimensional Data

**Problem**

Large number of player attributes.

**Solution**

Applied PCA for dimensionality reduction.

---

### 2. Missing Values

**Problem**

Several attributes contained missing entries.

**Solution**

Used appropriate imputation techniques.

---

### 3. Feature Correlation

**Problem**

Many football skills are highly correlated.

**Solution**

Used tree-based models and PCA to reduce the impact.

---

### 4. Cluster Selection

**Problem**

Determining the optimal number of player groups.

**Solution**

Used Elbow Method and Silhouette Analysis.

---

### 5. Model Overfitting

**Problem**

Complex models may memorize training data.

**Solution**

Train-test split and model comparison to ensure generalization.

---

## Technologies Used

### Programming Language

* Python

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-Learn

### Clustering

* K-Means
* PCA

### Development Environment

* Jupyter Notebook

---

## Business & Football Insights

This analysis can help:

* Scout player talent
* Compare players objectively
* Identify player archetypes
* Estimate player market value and quality
* Support transfer and recruitment decisions
* Understand player development patterns

---

## Future Improvements

Potential enhancements include:

* XGBoost and LightGBM implementation
* Advanced hyperparameter tuning
* Interactive dashboards using Streamlit
* SHAP explainability analysis
* Deep learning approaches
* Multi-season FIFA player trend analysis

---

## Conclusion

This project demonstrates an end-to-end football analytics workflow using FIFA 20 player data. Through exploratory analysis, clustering, and machine learning, meaningful insights were extracted about player characteristics, development patterns, and performance drivers. The resulting models and visualizations provide valuable support for football scouting, recruitment, and player evaluation.
