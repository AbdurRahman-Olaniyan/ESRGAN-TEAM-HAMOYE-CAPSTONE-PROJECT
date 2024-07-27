# ESRGAN-TEAM-HAMOYE-PROJECT
Data Science and Generative AI Project on educational Infrastructure
# ESRGAN-TEAM-HAMOYE-CAPSTONE-PROJECT
# Unlocking Potential: Exploring Factors in Student Success

## Introduction
This study investigates factors influencing educational outcomes using PISA Scores as a metric and target variable. The predictors include:

- Pupil-Teacher Ratio
- Annual Teacher Salary in USD (adjusted for ppp) 
- Government Expenditure on Education (% of Total)
- Shortage of Learning Materials Index

The study collected data from 86 countries with the aim of prescribing recommendations and policies to improve international education systems.

## Methodology
**Data Collection**: The study datasets were downloaded from OECD (https://www.oecd.org/en/data.html) and World Bank (https://data.worldbank.org/)
**Data Cleaning**: 
- Dropped duplicated data points
- Dropped Redundant and collinear variables 
- Set every variable to the correct data format
- Handled missing values

**Feature Engineering**: 
- Created "Spending Efficiency" feature (Ratio of PISA Scores to Govt expenditure on education)
- Created "Single PISA Score" feature (mean of Math, Reading and Science PISA Scores)

## Exploratory Data Analysis
- Performed descriptive analysis, distribution analysis, unsupervised statistical learning, and correlation analysis

![Distribution_Histogram](https://github.com/user-attachments/assets/6466eca9-bc57-42ae-a970-187061705b8f)

## Unsupervised Statistical Learning
- Trained a K-Means clustering algorithm to study the bimodal distribution of PISA Scores
- Revealed two clusters of countries: Cluster A with stronger education systems than Cluster B

![Cluster](https://github.com/user-attachments/assets/0568dc15-2d9a-4583-9d11-1c56e36a94dc)

![Distribution_Boxplot](https://github.com/user-attachments/assets/7f04c8ad-01a9-410f-ade2-de435ba8a644)

![Corr_ScaterPlot](https://github.com/user-attachments/assets/4d89724e-8472-4d56-99ec-1dcee72b2327)

![SpendingEff](https://github.com/user-attachments/assets/804b3728-c6d6-4cf6-8a7a-43e7b9da7dd1)

![CorrMap](https://github.com/user-attachments/assets/ce79a296-19b1-4529-914e-2f7f2dc39509)


## Key Findings
1. **Top performers**: Singapore, China, Korea, Finland, Japan
   **Bottom performers**: Cambodia, Dominican Republic, Philippines, Uzbekistan, Kosovo
2. **PISA Scores**: Bimodal distribution with higher cluster consisting of most European, North American, Australian, East Asian       countries and lower cluster consisting of most South American, West Asian, South East Asia, African countries
3. **Correlations**:
   - Teacher Salary and PISA Score: Strong positive (0.61)
   - Pupil-Teacher Ratio and PISA Score: Strong negative (-0.51) 
   - Government Expenditure and PISA Score: Negative (-0.35)
4. **K-Means Clustering**:
   - Cluster A (Higher performers): Lower pupil-teacher ratio, better learning materials, higher teacher salaries, lower government spending

## Policy Recommendations
**For Underperforming Countries**:
1. Reduce class sizes
2. Invest in teacher development and competitive salaries
3. Ensure access to learning resources
4. Improve spending efficiency
5. Foster a culture of learning

**For High-Performing Countries**:
1. Share best practices
2. Address equity gaps
3. Promote innovation in education

## Data Science AI Assistant
- Developed a data science AI assistant powered by RAG
- Key components: LLMs, Embedding Models, Document, Vector Database, RAG Framework
- Utilized libraries like langchain, anthropic, voyageai, google-genai, pypdf, faiss-cpu, streamlit, python
- Parsed document, created vector retriever, designed prompts, created history-aware retriever and retrieval chain
- Built UI with Streamlit and deployed on local server

  ![RAG AI UI](https://github.com/user-attachments/assets/344a4b91-552d-4e20-b1e9-b6d52545ca31)


## Conclusion
- Stronger international cooperation amongst nations can help improve global education systems
- Every country should implement data-driven decision making
