# Минипроект по работе с временем и сводными таблицами
В проекте я отвечаю на вопросы бизнеса, работая с данными о времени и дате
## Задачи
1. Загрузим датасет transaction_data.csv. Проверим размер таблицы, типы переменных, число пропущенных значений и описательную статистику.
2. Какие значения находятся в колонке transaction? Сколько наблюдений относятся к тому или иному уровню? Визуализируем результат с помощью барплота. Подумаем, как можно улучшить график.
3. Сколько транзакций завершились ошибкой?
4. Сколько успешных транзакций осуществил каждый из пользователей? Построим гистограмму распределения числа успешных транзакций.
5. Коллега прислал обновленные данные. Построим сводную таблицу user_vs_minute_pivot, где в качестве столбцов будут использованы имена пользователей, строк – минуты, значений – число совершенных операций в указанную минуту. Пропущенные значения заполним нулями.
6. Разбираемся,  есть ли в данных ошибка, или же всё хорошо.
7. Исправляем ошибку и сохраняем правильное число минут, прошедших с начала дня, в колонку true_minute.
