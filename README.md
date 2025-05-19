# Exploratory-Data-Analysis-EDA-
#  Titanic Dataset - Exploratory Data Analysis (EDA)

This project conducts **exploratory data analysis (EDA)** on the Titanic dataset using Python libraries such as **Pandas**, **Seaborn**, and **Matplotlib**. The goal is to extract insights and understand the data to inform future modeling tasks.

---

##  Project Objective

The objective is to explore the Titanic dataset to uncover meaningful patterns, detect anomalies, and draw conclusions using statistical summaries and visualizations. This analysis supports better understanding and feature selection for predictive modeling.

---

## Analysis Summary

### Dataset Overview

- The dataset includes demographic and personal data of Titanic passengers.
- Key features:
  - `Survived`: Target variable (0 = No, 1 = Yes)
  - `Pclass`, `Sex`, `Age`, `Fare`, `Embarked`, `SibSp`, `Parch`, `Cabin`

### 📈 Key Findings

1. **Survival Count**
   - More passengers died than survived.
   - Indicates class imbalance, important for predictive modeling.

2. **Passenger Class Distribution**
   - Most passengers were in **3rd class**, followed by **1st** and **2nd**.
   - Uneven class distribution; 3rd class passengers were the majority.

3. **Age Distribution**
   - Most passengers were **young adults (20–40 years)**.
   - The distribution is **right-skewed**, with fewer elderly passengers.

4. **Survival by Gender**
   - **Females had a higher survival rate** than males.
   - Suggests “**women and children first**” evacuation policy was followed.

5. **Correlation Matrix (Heatmap)**
   - `Survived` correlates positively with `Fare` and negatively with `Pclass`.
   - Moderate correlation between `SibSp` and `Parch` (multicollinearity warning).

6. **Missing Data**
   - The `Cabin` column contains many missing values.
   - The `Age` column has some missing values and may need imputation.

---

##  Visualizations Used

| Plot Type    | Purpose |
|--------------|---------|
| **Countplot** | Compare categorical features like Sex, Pclass, Survived |
| **Histogram** | Understand distribution of Age and Fare |
| **Boxplot**   | Compare Age and Fare with survival outcome |
| **Heatmap**   | Visualize correlations between numeric features |
| **Pairplot**  | Explore pairwise relationships by survival status |

---

##  EDA Concepts Explained

### 1. What is EDA?
Exploratory Data Analysis is a critical step in the data science process to:
- Understand data structure and patterns
- Identify outliers, anomalies, and trends
- Guide data preprocessing and feature selection

### 2. Common Correlation Plots
- **Heatmap**: Color-coded correlation matrix
- **Pairplot**: Histograms and scatter plots showing variable relationships

### 3. Handling Skewed Data
- Use `.skew()` and histograms to detect skew
- Apply transformations: `log`, `sqrt`, or `Box-Cox`
- Use binning or robust models if needed

### 4. Detecting Multicollinearity
- **Correlation Matrix**: Visual inspection
- **Variance Inflation Factor (VIF)**: VIF > 5–10 indicates multicollinearity

### 5. Types of Analysis
| Type           | Description                          |
|----------------|--------------------------------------|
| **Univariate** | Analysis of a single variable (e.g., Age) |
| **Bivariate**  | Two-variable analysis (e.g., Sex vs Survived) |
| **Multivariate** | Multiple variables (e.g., Pclass, Age, Fare vs Survived) |

### 6. Heatmap vs Pairplot
- **Heatmap**: Focused, color-coded matrix of correlation coefficients
- **Pairplot**: Comprehensive pairwise comparison of features, with survival-based coloring

### 7. Summarizing Insights
- Use bullet points to highlight trends
- Support insights with visuals
- Focus on patterns that help improve predictive accuracy

---

##  Tools Used

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas**
- **Seaborn**
- **Matplotlib**

---
##  Conclusion

Exploratory data analysis of the Titanic dataset reveals critical insights into **passenger survival**, influenced heavily by **gender, class, age**, and **fare**. These findings guide data preprocessing, feature engineering, and the design of predictive models in future stages.

---

