# Мини-проекты по работе cо скользящим средним и интеративными графиками
## Задачи [мини-проекта 1](https://github.com/belladzhu/python_projects/blob/main/mini-projects-window/mini-project-ads.ipynb)
Работа с данными взаимодействий с рекламными объявлениями на некоторой площадке за 6 дней. И таблица с характеристиками рекламных клиентов (тех, кто разместил эти объявления)
1. Разберемся с распределением количества показов и кликов. Посчитаем среднее количество показов и среднее количество кликов на объявления за весь период.
2. Нарисуем график распределения показов на объявление за весь период.
3. Посчитаем скользящее среднее показов с окном 2. Проверим значение скользящего среднего за 6 апреля 2019 года.
4. Скользящее среднее часто используется для поиска аномалий в данных. Попробуем нанести на один график значения арифметического среднего по дням и скользящего среднего количества показов. Посмотрим в какой день наблюдается наибольшая разница по модулю между арифметическим средним и скользящим средним? Дни, в которых скользящее среднее равно NaN, не учитываем. 
5. *Напишем функцию, которая найдет проблемное объявление (с наибольшим/наименьшим количеством показов) в день, в который была замечена самая большая по модулю аномалия. 
6. Теперь подгрузим данные по рекламным клиентам и найдем среднее количество дней от даты создания рекламного клиента и первым запуском рекламного объявления этим клиентом.
7. Вычислим конверсию из создания рекламного клиента в запуск первой рекламы в течение не более 365 дней. Ответ в процентах и с округлением до сотых. (Фильтровать будем по значению в формате pd.Timedelta(365, unit='d'))
8. Разобъем наших клиентов по промежуткам от создания до запуска рекламного объявления, равным 30. Определим, сколько уникальных клиентов запустили свое первое объявление в первый месяц своего существования (от 0 до 30 дней). Список промежутков для метода pd.cut – [0, 30, 90, 180, 365]
9. Выведем на интерактивный график эти категории с количеством уникальных клиентов в них.
## Задачи [мини-проекта 2](https://github.com/belladzhu/python_projects/blob/main/mini-projects-window/avocado.ipynb)
Работа с данными от Hass Avocado Board с использованием rolling 🥑 \
Посмотрим динамику цен на авокадо в США. В датафрейме находятся данные не за каждый день, а за конец каждой недели. Для каждой даты есть несколько наблюдений, отличающихся по типу авокадо и региону продажи. Нас это разделение не интересует, поэтому в avocado_mean мы сначала запишем агрегированные данные.
1. Посчитаем скользящее среднее цены авокадо с окном равным 3
2. Посмотрим, как изменится график в зависимости от выбранного размера окна.
3. Посчитаем экспоницеальное скользящее среднее
4. Импортируем полные данные. Для авокадо типа organic в Чикаго посчитаем скользящее среднее с окном 4 и экспоненциальное скользящее среднее с параметром span=4. Построим графики, а затем заполним пропуски.
5. Работа с данными по опозданиям в заключении сделок
6. Делим время на промежутки (на 3 интервала: 'less than 1 day' – время от 0 до 1 дня; '1-2 days' – от 1 до 2 дней; '2-3 days' – от 2 до 3 дней; 'more than 3 days' – больше 3 дней)
7. Строим интерактивный барплот с тем, насколько часто задерживаются сделки. 