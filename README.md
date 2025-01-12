# Evaluating Factors Influencing PISA Test Reading Scores

## Project Overview
This project analyzes the PISA (Program for International Student Assessment) dataset to uncover factors influencing the reading performance of 15-year-old students worldwide. By examining demographics, parental education, school characteristics, and student behavior, this study aims to provide actionable insights for educators and policymakers to enhance literacy and academic outcomes.

---

## Dataset Description
The dataset includes key features related to students' backgrounds and performance. Some notable variables are:
- **grade**: Student grade level (e.g., 10th grade for most 15-year-olds in the US).
- **male**: Gender indicator (1 = male, 0 = female).
- **raceeth**: Composite score representing race/ethnicity.
- **preschool**: Whether the student attended preschool (1 = yes, 0 = no).
- **expectBachelors**: Whether the student expects to earn a bachelor's degree (1 = yes, 0 = no).
- **parental education**: Indicators for parents' high school or bachelor’s completion (1 = yes, 0 = no).
- **readingScore**: The student's reading score on a 1000-point scale.
- **school characteristics**: Information about school type, location, and resources.

For a full list of features, please refer to the project files.

---

## Workflow

### 1. Data Preprocessing
- **Handling Missing Values**:
  - Numerical columns: Filled missing values with the median.
  - Categorical columns: Used the mode (e.g., `raceeth`) for imputation.
- **Categorical Transformation**:
  - Applied one-hot encoding to categorical variables for compatibility with statistical models.

---

### 2. Exploratory Data Analysis (EDA)
- **Correlation Matrix**:
  - Generated a heatmap to visualize relationships between variables.
- **Data Visualizations**:
  - Used bar charts, scatter plots, and box plots to explore key relationships.

---

### 3. Hypothesis Testing
- **T-Tests**:
  - Evaluated the impact of gender on reading scores.
  - Finding: Female students significantly outperform male students (p < 0.05).
- **ANOVA**:
  - Assessed differences between public and private school reading performance.
  - Finding: Private school students outperform public school students (p < 0.05).

---

### 4. Regression Analysis
- Conducted multiple linear regression to identify significant predictors of reading scores:
  - Parental education, gender, and study habits were strong predictors.
  - Analyzed coefficient significance (p-values) and confidence intervals.

---

### 5. Conclusions and Recommendations
**Key Findings**:
- **Gender**: Female students outperform males in reading.
- **School Type**: Private school students perform better, highlighting potential resource disparities.
- **Parental Education**: Higher parental education significantly boosts student outcomes.
- **Study Habits**: Reading for pleasure improves scores.

**Recommendations**:
- Implement programs encouraging reading among boys.
- Foster parental engagement through workshops and resources.
- Invest in public school improvements, focusing on equitable resource distribution.

---

