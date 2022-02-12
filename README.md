# New_York_City_Taxi_Trip_Duration
Подробный блокнот со всеми этапами построения модели и с пояснениями находится в файле "Taxi_Trip_Duration.ipynb"

## Задача

Соревнование на Kaggle - https://www.kaggle.com/c/nyc-taxi-trip-duration/overview. Нужно предсказать продолжительность поездки такси по следующим признакам:

- id - идентификатор поездки
- vendor_id - код провайдера, от которого пришла информация о поездке
- pickup_datetime - время старта поездки
- dropoff_datetime - время окончания поездки
- passenger_count - число пассажиров (вводится водителем)
- pickup_longitude - долгота точки посадки
- pickup_latitude - широта точки посадки
- dropoff_longitude - долгота точки высадки
- dropoff_latitude - долгота точки высадки
- store_and_fwd_flag - равно Y, если информация о поездке какое-то время хранилась в памяти таксометра из-за отсутствия связи; иначе принимает значение N
- trip_duration - продолжительность поездки в секундах

## Результаты

Наилучший результат был достигнут с помощью метода градиентного бустинга. Удалось уменьшить ошибку в среднем до 3.7 минут на метрике MAE и до 5.9 минут на метрике RMSE. При этом константные предсказания до обработки данных и выделения признаков были следующими: MAE = 9.5 минут, а RMSE = 87.5 минут (из-за большого количества выбросов).
