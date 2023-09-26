# Predicting_taxi_orders
В данном проекте мы решаем задачу предсказания количества заказов такси по часам. В качестве метрики выбрана RMSE, причём значение метрики на тестовой выборке не должно превышать 48. 


Исходные данные представляют собой файл формата .csv, содержащий временные ряды из двух столбцов - времени в формате datetime и количеством заказов в это время.


Для повышения точности предсказаний мы обогатили датасет синтетическими признаками (значения таргета с временным лагом, скользящее стреднее).


Данные были разбиты на выборки и нормализованы.


Для обучения были выбраны модели Ridge Regression, GradientBoostingRegressor, RandomForestRegressor. Для моделей Ridge Regression и GradientBoostingRegressor был осуществлен подбор гиперпараметров (alpha и learning_rate соответственно).


Наилучшие результаты удалось получить на модели RandomForestRegressor, RMSE = 42.
