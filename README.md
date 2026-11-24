# student-performance-analysis
DTS 201 group project predicting course pass/fail using student assessment scores.

## Project summary

## Data set
We got the CSV from Mendeley Data: https://data.mendeley.com/datasets/vzfyk22fhn/4

## Data preparation

## Exploratory Data Analysis

We used Pandas and Matplotlib to examine the dataset’s structure,
summarise assessment scores, visualise performance categories and
explore relationships between assessment components.

The analysis included descriptive statistics, category counts, bar
charts, a histogram of final examination marks, correlation analysis,
a scatter plot, and comparisons of average assessment scores across
performance categories.

### Key Findings

- The dataset contained 560 student records and 12 columns, with no
  missing values or duplicate records.
- Distinction was the most common original performance category,
  containing 301 students.
- The average total score was approximately 71.20 out of 100.
- There were 41 failure records and 519 passing records, making the
  classification task imbalanced.
- Project and presentation scores had a positive correlation of
  approximately 0.515.
- Midterm and final examination scores had a positive correlation of
  approximately 0.290.

Assessment components have different maximum marks, so their raw
averages should not be directly compared as performance percentages.
