🌍 AI Job Market Analysis 2025
Author: Anh Linh Le

📌 Executive Summary
This project analyzes the global AI job market in 2025 using a curated dataset of job postings. It aims to identify the key factors driving AI job salaries, trends in technical skill demand, and diversity and benefit signals across industries and regions. Through feature engineering, regression modeling, and trend analysis, we provide actionable insights for job seekers, employers, and policymakers.

📚 Table of Contents
Introduction & Problem Statement

Data Description

Methods & Analysis Pipeline

Results & Visualizations

Salary Modeling

Skill Demand Trends

Benefits & D&I Analysis

Conclusions & Recommendations

Limitations & Future Work

🧠 Introduction & Problem Statement
The explosive growth of AI has resulted in a competitive global job market. Employers, job seekers, and governments need clarity on what drives AI job salaries, which skills are most in demand, and how equitable and attractive AI roles are across regions and sectors.

Goals:

Predict AI job salaries using job, skill, and company attributes

Track skill demand evolution by geography and time

Analyze diversity, education, benefits, and work arrangement patterns

📊 Data Description
Source: Aggregated dataset of global AI job postings (2024–2025)
Size: 15000 entries

Key Fields:

job_id, job_title, company_name, posting_date, application_deadline

salary_usd, salary_currency, salary_usd_norm

experience_level, years_experience, education_required

company_location, company_size, industry

required_skills, skills_list, skill_*

remote_ratio, is_remote, is_hybrid, is_onsite

benefits_score

Preprocessing:

One-hot encoding of categorical variables

Skill extraction from free-text fields

Feature normalization

🧪 Methods & Analysis Pipeline
✅ 1. Exploratory Data Analysis
Checked distributions, missing values, and outliers

⚙️ 2. Feature Engineering
Encoded categorical features 

Normalized salary data

Created binary flags for remote/hybrid/onsite roles

🤖 3. Salary Modeling
Trained Linear Regression, Random Forest, and XGBoost models

Evaluated performance using MAE, RMSE, and R²

📈 4. Skill Trend Analysis
Exploded skill lists

Aggregated by month and country

Visualized top trending skills

💼 5. Benefits & D&I Analysis
Grouped benefits_score by industry and work arrangement

Analyzed education requirements across postings

📊 Results & Visualizations
4.1 Salary Modeling
Model	MAE	RMSE	R²
Linear Regression	0.0933	0.1205	0.6467
Random Forest	0.0947	0.1242	0.6248
XGBoost	0.0993	0.1303	0.5872

💡 Best Model: Linear Regression, explaining ~65% of salary variance.

🔑 Top Salary Drivers (Feature Importance - Random Forest):

![image](https://github.com/user-attachments/assets/cc1b93e8-17c1-462b-b18e-7f2c8d109cc8)


4.2 Skill Demand Trends
🌐 Top 20 In-Demand AI Skills (Global):

![image](https://github.com/user-attachments/assets/0026b32d-a477-4e75-9df4-6282b67ea515)





📊 Trends in Australia vs US vs India (2024–2025):


![image](https://github.com/user-attachments/assets/cd23bc99-1d3d-462f-83cd-4263c77dd488)







4.3 Benefits & D&I Analysis
🏢 Average Benefits Score by Industry:

![image](https://github.com/user-attachments/assets/2211bb8a-c352-47c3-b919-2c4dfaf5e90f)


Tech and Finance sectors lead in benefits

Retail and Government sectors lag behind




🏠 Work Arrangement vs. Benefits:


![image](https://github.com/user-attachments/assets/17f13a30-f596-4210-929c-35c6d45744f0)


Remote roles show slightly higher average benefits




🎓 Education Requirements:

![image](https://github.com/user-attachments/assets/f2c14edb-5fd5-4a19-946d-00693131104b)


Most jobs require Bachelor’s

Master's and PhDs are less common but linked to higher pay


✅ Conclusions & Recommendations
💰 Salary Drivers
Years of Experience: Strongest influence

Technical Skills: Deep learning & MLOps (e.g., TensorFlow, Kubernetes) command premium

Company Size & Industry: Bigger firms in Tech, Finance, Healthcare pay more

Work Arrangement: Remote/hybrid roles offer slightly better compensation

Education: Grad degrees help but less than skills & experience

🎯 Job Seeker Advice
Upskill in Deep Learning, Cloud (GCP, Azure), and MLOps

Apply to large firms in high-paying sectors

Showcase project experience and key AI tools

Don’t overlook remote/hybrid options

🏢 Employer Suggestions
Competitive salaries required for top AI talent

Benefits and flexibility matter

Upskilling internal staff in AI pays off

🧩 Limitations & Future Work
Limited to job posting data (not actual hiring outcomes)

Region-level skill analysis may miss local nuances

Future: Integrate real-world hiring data & candidate outcomes


