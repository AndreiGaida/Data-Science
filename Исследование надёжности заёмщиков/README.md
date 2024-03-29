# Исследование надежности заемщиков
## Описание проекта
Заказчик — кредитный отдел банка. Нужно разобраться, влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. Входные данные от банка — статистика о платёжеспособности клиентов.
Результаты исследования будут учтены при построении модели кредитного скоринга — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.
## Описание данных
- children — количество детей в семье
- days_employed — общий трудовой стаж в днях
- dob_years — возраст клиента в годах
- education — уровень образования клиента
- education_id — идентификатор уровня образования
- family_status — семейное положение
- family_status_id — идентификатор семейного положения
- gender — пол клиента
- income_type — тип занятости
- debt — имел ли задолженность по возврату кредитов
- total_income — ежемесячный доход
- purpose — цель получения кредита
## Используемые библиотеки 
pandas
## Вывод по итогам исследования
Из даннного исследования мы можем сделать вывод, что люди берущие кредит на оперции с недвижимостью более ответственно подходят к задолженности(7.26%). Так же люди берущие кредит для проведения свадьбы более ответственно подходят к выполнению своих обязательств(7.91%) в сравнениями с другими категориями: 'операции с автомобилями'(9.35%), 'получени образования'(9.25%).
