# Итоговый проект. Агентство недвижимости

## Оглавление  
[1. Описание проекта](https://github.com/eco189/Final_project/blob/main/README.md#Описание-проекта)    
[2. Краткая информация о данных](https://github.com/eco189/Final_project/blob/main/README.md#Краткая-информация-о-данных)  
[3. Этапы работы над проектом](https://github.com/eco189/Final_project/blob/main/README.md#Этапы-работы-над-проектом)  
[4. Результат](https://github.com/eco189/Final_project/blob/main/README.md#Результат)    
[5. Инструкция по запуску Docker-контейнера](https://github.com/eco189/Final_project/blob/main/README.md#Инструкция-по-запуску-Docker-контейнера) 

### Описание проекта    
Агентству недвижимости необходимо разработать сервис для предсказания стоимости домов на основе истории предложений.

:arrow_up:[к оглавлению](https://github.com/eco189/Final_project/blob/main/README.md#Оглавление)


### Краткая информация о данных
Данные о домах находятся в хранилище Google Диск. Название файла: data.csv Разделитель: sep=',' Ссылка: https://drive.google.com/file/d/11-ZNNIdcQ7TbT8Y0nsQ3Q0eiYQP__NIW/view?pli=1
  
:arrow_up:[к оглавлению](https://github.com/eco189/Final_project/blob/main/README.md#Оглавление)

### Этапы работы над проектом
- Исследование структуры данных
- Преобразование данных
- Исследование зависимостей в данных
- Очистка данных
- Обучение на разных моделях

:arrow_up:[к оглавлению](https://github.com/eco189/Final_project/blob/main/README.md#Оглавление)


### Результат:
- Получена обученная модель. Модель CatBoostRegressor показала лучший результат по сравнению с остальными. Ошибка МАРЕ на тестовой выборке составила 16,54 %.   
- На основе данной модели разработан сервис для предсказания стоимости домов.
- Docker-контейнер с данным сервисом был собран и загружен на Docker Hub.

:arrow_up:[к оглавлению](https://github.com/eco189/Final_project/blob/main/README.md#Оглавление)


### Инструкция по запуску Docker-контейнера:  
1. Скачать образ с Docker Hub с помощью команды:    
docker pull eco189/final_project_server_image  
2. Запустить контейнер командой:  
docker run -d -p=80:80 eco189/final_project_server_image  
3. Через браузер зайдём по адресу http://localhost
4. В поля в левой колонке вводим данные, выбирая из выпадающего списка, в поля в правой колонке вводим данные вручную.
4. Нажимаем на "Predict" и получаем предсказание цены.

:arrow_up:[к оглавлению](https://github.com/eco189/Final_project/blob/main/README.md#Оглавление)