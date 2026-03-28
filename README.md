# Future ML Projects Portfolio

This repository contains various machine learning and data science tasks focused on predictive modeling and NLP.

## Task 1: Store Sales - Time Series Forecasting
**Objective**: Predict grocery sales for Corporation Favorita using historical data from the Kaggle Store Sales Competition.
- **Model**: Random Forest Regressor
- **Key Features**: Time features (Year, Month, Day), Lag features (Sales_Lag1).
- **Performance**: Achieved a Mean Absolute Error (MAE) of **$30,652.10**.

## Task 3: Resume Ranking System (NLP)
**Objective**: Automate the recruitment process by ranking resumes based on their similarity to a specific job description.

### Methodology
1. **Data Loading**: Loaded a dataset of 2,484 resumes categorized by industry.
2. **Preprocessing**: Normalized text (lowercase, removed URLs, special characters, and extra spaces).
3. **Similarity Scoring**: Used **TF-IDF Vectorization** to convert text into numeric vectors and **Cosine Similarity** to calculate the match percentage between resumes and the job description.
4. **Skill Matching**: Implemented a custom extraction function to identify present and missing skills for each candidate.

### Top 10 Candidates (Sample Output)
Below are the top-ranking candidates for a Software Engineer job description (Python, SQL, ML, NLP, AWS).

| Rank | ID | Category | Match Score (%) | Skills Found |
|------|----|----------|-----------------|--------------|
| 1 | 20824105 | INFORMATION-TECHNOLOGY | 14.49 | python, aws |
| 2 | 12011623 | ENGINEERING | 13.02 | python, sql, machine learning |
| 3 | 51588273 | ENGINEERING | 11.89 | sql, java |
| 4 | 83816738 | INFORMATION-TECHNOLOGY | 11.28 | sql, aws, java |
| 5 | 10624813 | ENGINEERING | 10.74 | python, sql, aws, java |
| 6 | 27419236 | DIGITAL-MEDIA | 9.95 | sql |
| 7 | 30863060 | CONSULTANT | 9.82 | sql, java |
| 8 | 28126340 | INFORMATION-TECHNOLOGY | 9.59 | sql, java |
| 9 | 21297521 | BANKING | 9.51 | sql, nlp, aws, java, docker, kubernetes |
| 10 | 21156767 | CONSULTANT | 9.17 | python, sql, machine learning, java |


### Key Insights
- The **Information-Technology** and **Engineering** categories showed the highest average fit scores, as expected for a technical role.
- The TF-IDF model successfully captured keyword relevance while the similarity scoring allowed for granular ranking beyond simple keyword count.

---

