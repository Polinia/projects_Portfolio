
# Project #8: Car Price prediction Part2 (Neural networks, Computer Vision)
https://www.kaggle.com/polinafedosova/carpriceprediction2-polina-aleksandr-27b9a9
Public Score on Kaggle.com: 10.77901
## Goal:
to predict car price by its characteristics, text description or picture.
# Objectives:
- Let's build a "naive" / baseline model that predicts the price by model and year of manufacture (we will compare other models with it)
- tp process and normalize features
- to make the first model based on gradient boosting using CatBoost
- to make a second model based on neural networks and compare the results
- to build a multi-input neural network to analyze tabular data and text at the same time
- to add image processing to the multi-input network
- to build an ensemble of gradient boosting and neural network (averaging their predictions)
# Conclusion:
we carried out all the necessary work on data preparation, their analysis, processing and preparation for further work . The dataset is cleared of duplicates and outliers, normalization is performed, classical methods of coding categorical features were used. Additional features have been created. According to the results of the analysis, some of the features, including those based on correlation analysis, deleted. Classical language processing methods were used. We used tokenization and lemmatization in the model.
While working with images, we used our own augmentation code based on the albumentation library. Experiments have been carried out with other typical EfficientNet models,
some of which led to retraining. The Learning Rate adjustment was applied. Fine-tuning and Transfer Learning were also used.
As a result of blending, we managed to achieve good results of the metric 10.77901.

# skillfactory_rds

* Название комманды на Kaggle: Polina&Aleksandr
* Cостав комманды: [Polina Rudakova](https://github.com/Polinia), [Aleksandr](https://github.com/AleksandrBychkov?tab=overview&from=2021-04-01&to=2021-04-14)
* Ссылка на ноутбук в Kaggle: https://www.kaggle.com/polinafedosova/carpriceprediction2-polina-aleksandr-27b9a9

Задача
-----------
https://www.kaggle.com/c/sf-dst-car-price-prediction-part2

Предсказать стоимость автомобиля по его характеристикам, текстовому описанию или картинке

Описание признаков
------------------------
* bodyType - категориальный
* brand - категориальный
* color - категориальный
* description - текстовый
* engineDisplacement - числовой, представленный как текст
* enginePower - числовой, представленный как текст
* fuelType - категориальный
* mileage - числовой
* modelDate - числовой
* model_info - категориальный
* name - категориальный, желательно сократить размерность - не используется (комбинация других столбцов)
* numberOfDoors - категориальный
* price - числовой, целевой
* productionDate - числовой
* sell_id - изображение (файл доступен по адресу, основанному на sell_id)
* vehicleTransmission - категориальный
* vehicleConfiguration — не используется (комбинация других столбцов)
* Владельцы - категориальный
* Владение - числовой, представленный как текст
* ПТС - категориальный
* Привод - категориальный
* Руль - категориальный

В результате работы было достигнуто следующее:
--------------
Построили "наивную"/baseline модель, предсказывающую цену по модели и году выпуска (с ней сравнивали другие модели)

Обработали и отнормироавали признаки

Сделали первую модель на основе градиентного бустинга с помощью CatBoost

Сделали вторую модель на основе нейронных сетей и сравнили результаты

Сделали multi-input нейронную сеть для анализа табличных данных и текста одновременно

Добавили в multi-input сеть обработку изображений

Осуществили ансамблирование градиентного бустинга и нейронной сети (усреднение их предсказаний)

Выводы:
-------
Проведена вся необходимая работа по подготовке данных, их анализ, обработка и подготовка для дальнейшей работы. Датасет очищен от дубликатов и выбросов, выполнена нормализация, 
использовались классические методы кодирования категориальных признаков. Были созданы дополнительные признаки. По итогам анализа, часть признаков,
в том числе на основе анализа корреляции, удалена. Использовались классические методы обработки языка. В модели применялась токенизация и лемматизация.
При работе с изображениями использовался собственный код аугментации на основе библиотеки albumentation. Были проведены эксперименты с другими типовыми моделями EfficientNet, 
часть из которых приводила к переобучению. Применялась регулировка Learning Rate. Так же использовались Fine-tuning и Transfer Learning.
По итогам блендирования удалось достичь хороших результатов метрики 10.77901.

Структура репозитория
-----------------
В папке [data](https://github.com/Polinia/skillfactory_rds/tree/main/module_8/data) находятся файлы для скачивания:

* sample_submission.scv
* test.scv
* test.scv
* img
