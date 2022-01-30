Project #4. Credit Scoring
========================
## Objectives:
to build a scoring model for the bank's secondary clients that would predict the probability of a client's default. To do this, it will be necessary to determine the significant parameters of the borrower.

## Data Description:

![2022-01-30 (1)](https://user-images.githubusercontent.com/68026029/151710271-d29dae5b-c55b-4bd9-8bea-0c2a06981015.png)

# As a result of the work, the following were achieved:
* ROC AUC - 0.739
* Accuracy score - 0.6744
* F1-score - 0.6759
* MSE - 0.3256
* Recall score - 0.6782
* TP - 8707
* FP - 4278
* FN - 4191
* TN - 8831

## Conclusions:
We carried out a series of a standard manipulations on the selection of training models and the best hyperparameters. This made it possible to obtain decent and stable results in all parts of the sample.

# skillfactory_rds
* Название комманды на Kaggle: Polina&Aleksandr
* Cостав комманды: [Polina Rudakova](https://github.com/Polinia), [Aleksandr](https://github.com/AleksandrBychkov?tab=overview&from=2021-04-01&to=2021-04-14)


Public Score on Kaggle.com: 0.73822
------------
Задача
-----------
https://www.kaggle.com/c/sf-dst-scoring

Построить скоринговую модель для вторичных клиентов банка, которая бы предсказывала вероятность дефолта клиента. Для этого нужно будет определить значимые параметры заемщика.

Описание признаков
------------------------
* client_id - идентификатор клиента
* education - уровень образования
* sex - пол заемщика
* age - возраст заемщика
* car - флаг наличия автомобиля
* car_type - флаг автомобиля иномарки
* decline_app_cnt - количество отказанных прошлых заявок
* good_work - флаг наличия “хорошей” работы
* bki_request_cnt - количество запросов в БКИ
* home_address - категоризатор домашнего адреса
* work_address - категоризатор рабочего адреса
* income - доход заемщика
* foreign_passport - наличие загранпаспорта
* sna - связь заемщика с клиентами банка
* first_time - давность наличия информации о заемщике
* score_bki - скоринговый балл по данным из БКИ
* region_rating - рейтинг региона
* app_date - дата подачи заявки
* default - флаг дефолта по кредиту

В результате работы были достигнуты следующие показатели:
--------------
* ROC AUC - 0.739
* Accuracy score - 0.6744
* F1-score - 0.6759
* MSE - 0.3256
* Recall score - 0.6782
* TP - 8707
* FP - 4278
* FN - 4191
* TN - 8831

Выводы:
-------
Провели ряд стандартных манипуляций по подбору моделей обучения и лучших параметров. Это позволило получить достойные и стабильные на всех частях выборки результаты.

Структура репозитория
-----------------
В папке [data](https://github.com/Polinia/skillfactory_rds/tree/main/module_4/data) находятся файлы для скачивания:

* sample_submission.scv
* test.scv
* train.scv
