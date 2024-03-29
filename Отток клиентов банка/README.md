# Отток клиентов банка
## Описание проекта
Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Нам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.
Необходимо построить модель с предельно большим значением F1-меры, нужно довести метрику до 0.59.
Источник данных: https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling
## Описание данных
- RowNumber — индекс строки в данных
- CustomerId — уникальный идентификатор клиента
- Surname — фамилия
- CreditScore — кредитный рейтинг
- Geography — страна проживания
- Gender — пол
- Age — возраст
- Tenure — количество недвижимости у клиента
- Balance — баланс на счёте
- NumOfProducts — количество продуктов банка, используемых клиентом
- HasCrCard — наличие кредитной карты
- IsActiveMember — активность клиента
- EstimatedSalary — предполагаемая зарплата
- Exited — Целевой признак, факт ухода клиента

## Используемые библиотеки
pandas, numpy, matplotlib, sklearn

## Вывод 
- Была проверена на тестовой выборке модель случайного леса.
- Рассчитали значение F1-меры(0.6122448979591837) и AUC-ROC(0.8497593824902651) для случайного леса.
- Построили ROC-кривую для случайного леса.
- Параметры, дающие лучший результат: {n_estimators = 14, max_depth = 9}
- Лучше всего выравнивать через class_weight="balanced"

