# ML-7.4: Оптимизация гиперпараметров

## Оглавление  
[1. Описание проекта](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Описание-проекта)  
[2. Какой кейс решаем?](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Какой-кейс-решаем)  
[3. Краткая информация о данных](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Краткая-информация-о-данных)  
[4. Этапы работы над проектом](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Этапы-работы-над-проектом)  
[5. Результат](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Результат)    

### Описание проекта
Оптимизация гиперпараметров моделей логистической регрессии и случайного леса четырьмя способами: GridSeachCV, RandomizedSearchCV, Hyperopt, Optuna. Практика основана на датасете соревнования Kaggle [Predicting a Biological Response](https://www.kaggle.com/competitions/bioresponse/overview) (Прогнозирование биологического ответа).

:arrow_up:[к оглавлению](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Оглавление)


### Какой кейс решаем?
Необходимо предсказать биологический ответ молекул (столбец 'Activity') по их химическому составу (столбцы D1-D1776).

**Условия задания:**
- Предварительная обработка не требуется, данные уже закодированы и нормализованы.
- В качестве метрики используется F1-score.
- Необходимо обучить две модели: логистическую регрессию и случайный лес. Далее нужно сделать подбор гиперпараметров с помощью базовых и продвинутых методов оптимизации. Важно использовать все четыре метода (GridSeachCV, RandomizedSearchCV, Hyperopt, Optuna) хотя бы по разу, максимальное количество итераций не должно превышать 50.

:arrow_up:[к оглавлению](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Оглавление)


### Краткая информация о данных
Данные представлены в формате CSV. Каждая строка представляет молекулу.
- Первый столбец Activity содержит экспериментальные данные, описывающие фактический биологический ответ [0, 1]
- Остальные столбцы D1-D1776 представляют собой молекулярные дескрипторы — это вычисляемые свойства, которые могут фиксировать некоторые характеристики молекулы, например размер, форму или состав элементов

:arrow_up:[к оглавлению](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Оглавление)


### Этапы работы над проектом
Реализован подбор гиперпараметров для моделей логистической регрессии и случайного леса четырьмя способами:
- GridGridSeachCV
- RandomizedSearchCV
- Hyperopt
- Optuna

:arrow_up:[к оглавлению](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Оглавление)


### Результат:
- В результате оптимизации были улучшены метрики F1-score на тестовых выборках каждой модели. Метрика была улучшена после применения каждого из четырех методов оптимизации.   
- Блоки кода можно использовать в качестве готовых шаблонов при построении ML-моделей.

:arrow_up:[к оглавлению](https://github.com/eco189/ML-7.4_Optimization_of_hyperparameters/blob/main/README.md#Оглавление)
