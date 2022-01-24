# Fake/Real Job Posting Prediction
## Цель:
обучить модель классифицировать вакансии как реальные или мошеннические.

## Задачи:
Этот проект направлен на создание классификатора, который сможет идентифицировать поддельные и настоящие вакансии работ.Окончательный результат оценивается на основе нескольких моделей. Поскольку предоставленные данные имеют числовые и текстовые характеристики, одна из моделей будет использоваться для текстовых данных. Окончательная модель будет принимать любые соответствующие данные о вакансиях и давать окончательный результат, определяющий, является ли вакансия реальной или нет.

## Описание признаков:
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

## В результате работы было достигнуто следующее:
- датасет проверен на дубликаты и выбросы
- произведена очистка, извлечение чисел и текста из признаков
- произведен анализ данных
- измерена точность на экспериментах с удалением признаков
- создан бейзлайн, по которому сравнивались изменения в датасете
- использовались методы обработки языка, а именно очистка текста. В модели применялась токенизация и лемматизация
- получены результаты метрики таких моделей как: CatBoostClassifier, RandomForest, GradientBoosting, KNeighbors и Bi-Directional LSTM
