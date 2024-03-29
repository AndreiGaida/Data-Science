# Прогноз продаж в интернет-магазине
## Описание проекта
В интернет-магазине «Стримчик», который продаёт по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation). Необходимо выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании. Данные предоставлены до 2016 года.
## Описание данных
- Name — название игры
- Platform — платформа
- Year_of_Release — год выпуска
- Genre — жанр игры
- NA_sales — продажи в Северной Америке (миллионы проданных копий)
- EU_sales — продажи в Европе (миллионы проданных копий)
- JP_sales — продажи в Японии (миллионы проданных копий)
- Other_sales — продажи в других странах (миллионы проданных копий)
- Critic_Score — оценка критиков (максимум 100)
- User_Score — оценка пользователей (максимум 10)
- Rating — рейтинг от организации ESRB

## Используемые библиотеки
pandas, numpy, matplotlib, seaborn, scipy

## Вывод

Выяснили какие платформы лидируют по продажам, растут или падают.Самыми перспективными платформами являются PS4, XOne. Платформами которые теряют лидирующие поиции оказались 3DS,PS3,X360.

**Определили корреляцию платформ по отношению к оценке пользователей:**
- DS = 0.24(очень слабая корреляция)
- PC = -0.09(отсутствует корреляция)
- PS4 = 0.00(отсутствует корреляция)
- Wii = 0.35(слабая корреляция)
- Xbox = -0.04(очень слабая корреляция)
- другие платформы = -0.00(отсутствует корреляция)

**Определили корреляцию платформ по отношению к оценке критиков:**
- DS = 0.36(слабая корреляция)
- PC = 0.20(очень слабая корреляция)
- PS4 = 0.33(слабая корреляция)
- Wii = 0.38(слабая корреляция)
- Xbox = 0.35(слабая корреляция)
- другие платформы = 0.25(очень слабая корреляция)

Рассмотрели общее распределение игр по жанрам и выяснили,что наибольшие количество проданных игр у жанров "Shoter", "Sports", "Platform". 

**Составили портрет пользователя каждого региона:**
- Исследовали топ-5 самых популярных платформ в Северной Америке и выяснили, что платформы Microsoft(40%) и Sony(40%) являются самыми популярными.
- Исследовали топ-5 самых популярных платформ в Европе и выяснили, что потребитель чаще отдаёт предпочтение консоли от Sony(53%). Наибольшей популярностью пользуется PS4(36%).
- Исследовали топ-5 самых популярных платформ в Японии и выяснили, что 97% платформ являются японскими. Лидерство за 3DS(48%).
- Исследовали топ-5 самых популярных жанров в Северной Америке и выяснили, что в Северной Америке наибольшей популярностью пользуются Action(29%) и Shooter(25%) и суммарно занимают 54% рынка. Оставшуюся часть занимают жанры: Sports(15%), Role-Playing(11%), Misc(6%) и все остальные объединённые в общую группу(14%)
- Исследовали топ-5 самых популярных жанров в Европе и выяснили, что там практически аналогичные показатели с Северной Америкой: Action(30%), Shooter(22%), Sports(15%), Role-Playing(9%), другие жанры(17%). Отличием является появление на диаграмме жанра Racing(5%) на месте Misc.
- Исследовали топ-5 самых популярных жанров в Японии и выяснили, что наибольшей популярностью пользуются Role-Playing(36%). Заинтересованность в жанре Action сопоставима с другими регионами. Shooter имеет всего 5%, что существенно ниже чем в Северной Америке и Европе.
- Исследовали показатели диаграмм по рейтингу в Северной Америке и Европе и выяснили, что они очень схожи между собой. В Северной Америке чаще продаются видеоигры с рейтингом М, E10+ и T. В Европе чаще продаются видеоигры с рейтингом E. В Японии уже совершенно другие показатели, все вышеперечисленные категории продаются реже. Наибольшую долю рынка занимает видео игры с неизвестным рейтингом ESRB.

**Были проверены 2 гипотезы:**
- 1-ая: Средние пользовательские рейтинги платформ Xbox One и PC одинаковые;
- 2-я: Средние пользовательские рейтинги жанров Action (англ. «действие», экшен-игры) и Sports (англ. «спортивные соревнования») разные.

В результате использования специального метода для проверки гипотезы о равенстве среднего двух генеральных совокупностей по выборкам: гипотезу о равенстве средних пользовательский рейтингов по платформам XOne и PC удалось подтвердить. Гипотеза о равенстве средних пользовательских рейтингах жанров Action и Sports была отвергнута.

