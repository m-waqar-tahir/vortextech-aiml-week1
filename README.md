# Pakistan Student Employability Analysis

Vortex Tech AI & ML Internship 2026 — Week 1

## Overview

Data cleaning and exploratory data analysis on a dataset of academic, skill,
and career-readiness records for Pakistani university students. The goal was
to clean the raw data and explore which academic and skill factors relate
most strongly to employability outcomes.

## Dataset

`pk_student_employability_dataset.csv` — sourced from Kaggle, originally
50,000 student records. After removing rows with missing CGPA or attendance
and filling remaining gaps based on their likely meaning (e.g. unassessed
skills, no contributions, zero certifications), the cleaned dataset used for
analysis contains 47,839 records across 49 features.

## Files

- `student_employability_analysis.ipynb` — main notebook: data cleaning,
  exploratory data analysis, and a documentation report
- `pk_student_employability_dataset.csv` — raw dataset used
- `README.md` — this file

Running the notebook end to end also exports a cleaned copy of the dataset,
`pk_student_employability_cleaned.csv`, which is the file used as the
starting point for the Week 2 and Week 3 projects.

## Tech Stack

Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

## What the notebook covers

- Handling missing values with column-appropriate logic rather than a single
  blanket rule (e.g. skill columns filled as "Not Assessed", freelancing
  income filled with the median among actual freelancers)
- Removing duplicate records
- Descriptive statistics and distribution checks across demographics,
  academics, and skills
- Exploratory visualizations relating skills, internships, and academic
  performance to employability status
- A documentation report summarizing findings and recommendations

## How to run

1. Install dependencies:
   ```
   pip install pandas numpy matplotlib seaborn jupyter
   ```
2. Open the notebook:
   ```
   jupyter notebook student_employability_analysis.ipynb
   ```
3. Run all cells in order.

## Key findings

- After cleaning, the dataset contains 47,839 student records across 49
  features, drawn mainly from Punjab and Sindh, ages 17 to 31 with an
  average age of 21.
- Average CGPA is 2.91 out of 4.0, and higher CGPA is associated with a
  Highly Employable rating.
- Programming skill level and internship experience both show a clear link
  to employability — stronger skills and prior internships are associated
  with better outcomes.
- Average job readiness score is 93.1 out of 100, with most students rated
  as fully job ready.
- Expected salary averages about 75,966 PKR per month and rises with
  employability status.
- Numeric features show relatively weak correlation with each other,
  suggesting employability depends more on categorical and skill-based
  factors than on any single numeric measure.

## Recommendations

1. Encourage students with weaker programming skills to pursue structured
   upskilling, since skill level tracks closely with employability.
2. Promote internship placement programs, given the clear link between
   internship experience and stronger employability outcomes.
3. Track certifications, open-source contributions, and freelancing
   activity more consistently going forward, since these fields had high
   missing rates and may hold predictive value once reliably recorded.
4. Use employability status alongside job readiness score to help
   prioritize students who need additional career support.

## Status

✅ Completed

## Author

Muhammad Waqar Tahir
Vortex Tech AI & ML Internship 2026 — Week 1
