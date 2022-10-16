# Fake/Real Job Posting Prediction
## This project uses data from Kaggle:
https://www.kaggle.com/shivamb/real-or-fake-fake-jobposting-prediction

The aim of the project is to create a model for the classification of jobs as real or fraudulent.

## Data description:
- job_id- Identification number given to each job posting
- title - A name that describes the position or job
- location - Information about where the job is located
- department - Information about the department this job is offered by
- salary_range - Expected salary range
- company_profile - Information about the company
- description - A brief description about the position offered
- requirements - Pre-requisites to qualify for the job
- benefits - Benefits provided by the job
- telecommuting - Is work from home or remote work allowed
- has_company_logo - Does the job posting have a company logo
- has_questions - Does the job posting have any questions
- employment_type - 5 categories (Full-time, part-time, contract, temporary and other)
- required_experience - Can be: Internship, Entry Level, Associate, Mid-senior level, Director, Executive or Not Applicable
- required_education - Can be: Bachelor’s degree, high school degree, unspecified, associate degree, master’s degree, certification, some college coursework, professional, some high school coursework, vocational
- Industry - The industry the job posting is relevant to
- Function - The umbrella term to determining a job’s functionality
- Fraudulent - The target variable (0: Real, 1: Fake)

## As a result of the work, the following was achieved:
- dataset examined for duplicates and outliers
- data cleaning, extraction of numbers and text from features
- data analysis
- model evaluation
- a baseline was created, according to which changes in the dataset were compared
- natural language processing, stop-words cleaning, tokenization and lemmatization
- obtained the results of the metrics F1 for: CatBoostClassifier, RandomForest, GradientBoosting, KNeighbors and Bi-Directional LSTM

The best result got from CatBoostClassification:

![image](https://user-images.githubusercontent.com/68026029/151677930-14275d20-dd9f-48b4-96ca-3b3a64fb6406.png)

Bi-Directional LSTM:

![image](https://user-images.githubusercontent.com/68026029/151677952-4c79d181-eacc-40e9-ab81-d3efd1fdbfa2.png)
