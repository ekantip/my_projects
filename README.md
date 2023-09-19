### Привет!
### Меня зовут Екатерина, я аналитик данных.
В этой папке представлены мои проекты по анализу данных с помощью python. Разработка дашборда в Datalens.  

## Проект: [анализ продаж аттракционов](https://datalens.yandex/24ngfzukf4iar)
___Дано:___ заказчки - компания, продающая игры и аттракционы. Задача: разработать дашборд в Datalens для коммерческого директора. Отразить продажи, сезонность, выявить точки роста. Дизайн на мое усмотрение, основные метрики указаны в ТЗ, можно добавить свои. 

По ТЗ нужно отразить выручку в динамике, долю наличных и безналичных платежей. Отразить продажи в разрезе ценовых категорий игр. Расчитать средние данные (цена продажи, количество позиций в чеке, количество проданных услуг). Отразить продажи отдельно по объектам и по играм. Сделать сравнение период к кпериоду, рассчитать скользящее среднее.

___Что сделано:___
- разбила представление данных на три категории: картина в общем, средние показатели и детализация продаж. Развела их по разным вкладкам.
- выручку в динамике представила сразу в разбивке по видам платежа. Представила два вида диаграммы
- скользящее среднее и сравнение периодов разделила на две диаграммы
- разбивку по ценовым категориям представила в четырех диаграммах: круговой с долями, столбчатой с выручкой по категорям, столбчатой с количеством продаж по категорям, нормированной столбчатой
- средние показатели привязала к линейчатым графикам в динамике, чтобы можно было наглядно сравнить измения
- при обсуждении дашборда заказчик указал, что ему важно сравнивать объекты друг с другом и продажи период к периоду. Поэтому на вкладке с детализауией продаж создала таблицу сравнения и по объектам и по играм, рассчитала выручку, разницу с предыдущим периодом, % разницы, среднюю выручку и % возвратов
- также рассмотрены продажи по объектам и играм в различных разрезах

___Инструменты:___ Datalens.yandex.ru

___Примечание___ ссылка ведет на сайт с дашбордом на Datalens.yandex.ru. Данные по продажам намеренно размыты сгенерированными данными, так как в чистом виде являются коммерческой тайной и не подлежат раскрытию.

## Проект: [cегментация клиентов банка](https://github.com/ekantip/my_study_projects/blob/main/segmentation%20png.ipynb)
___Дано:___ в банке повысился отток клиентов (средний уровень составил 18%), необходимо провести сегментацию отточных клиентов для отдела маркетинга, для разработки предложения по удержанию клиентов.

___Что сделано:___ 
- провела короткий исследователтский анализ данных, получила общее представление о структуре данных о клиентах, определила средний уровень оттока
- поработала с пропусками: выявила связи между пропущенными и остальными данными на основе корреляций. Заменила пропущенные значения
- сравнила уровень оттока по каждому параметру клиента со средним уровнем оттока. Представила данные наглядно - подкрепила графиком.
- определила сегменты в параметрах, где уровень оттока выше среднего
- объединила клиентов по нескольким наиболее отточным признакам (уровень оттока выше в 2 раза и более), использовала циклы в python
- выдвинула две гипотезы и проверила их (критерий Манна-Уитни, z-критерий)
- общие выводы 

___Инструменты:___ python, pandas, scipy, numpy, plotly

___Примечание___ 1)Визуализация проекта выпонена с помощью библиотеки plotly, для ее отображения на github все графики выгружены в формат png, к сожалению качество картинки оставляет желать лучшего и она не интерактивна, но для составления общего впечатления о  работе этого достаточно. 2) Если проект долго грузится, пожалуйста, обновите страницу.

## Проект: [когортный анализ](https://github.com/ekantip/my_study_projects/blob/main/analysis%20of%20marketing%20indicators.ipynb)
___Дано:___ Задача — разобраться в причинах убытков рекламных компаний и помочь компании выйти в плюс.
Есть данные о пользователях, привлечённых с 1 мая по 27 октября 2019 года: лог сервера.
___Что сделано:___ 
- провела анализ расходов на маркетинг: анализ расходов по каналам привлечения, стоимость привлечения одного пользователя в канале (САС);
- оценила окупаемость рекламы: построила графики LTV и ROI, и графики динамики LTV, CAC и ROI 
- оценила окупаемость рекламы детально: с разбивкой по устройствам, по рекламным каналам, отдельно по странам и рекламным каналам
- выводы, рекомендации.

___Инструменты:___ python, pandas, numpy, matplotlib, seaborn

___Примечание___ Визуализация проекта выпонена с помощью библиотеки plotly, для ее отображения на github все графики выгружены в формат png, к сожалению качество картинки оставляет желать лучшего и она не интерактивна, но для составления общего впечатления о  работе этого достаточно. Если проект долго грузится, пожалуйста, обновите страницу.

## Проект: [воронка продаж + АВ-тестирование](https://github.com/ekantip/my_study_projects/blob/main/sales_funnel_AAB_test.ipynb)
___Дано:___ стартап, продающий продукты питания. Провели АВ-тестирование, чтобы понять как влияет на покупателей изменение шрифта в приложении. Нужно построить воронку продаж, проверить результаты теста статистическими методами. Тестов было три: между контрольными группами 246 и 247 (АА), им показали страницы без изменений. Группа №248 получила измененный шрифт в приложении. 
___Что сделано:___ 
- провела предобработку данных (поиск дубликатов, переименование столбцов)
- проверила корректность проведения теста (равномерность распределения пользователей по группам, пересечение пользователей между группами, сроки проведения теста)
- построила воронку продаж в разбивке по группам теста
- проверила различия долей статистичеким методом в группе А/А отдельно на каждом этапе воронки, чтобы убедиться что тест работает корректно
- проверила различия долей между группами 246 / 248 и 247 / 248
- общий вывод

___Инструменты:___ python, os, pandas, datetime, numpy, scipy, math, plotly

___Примечание:___ Визуализация проекта выпонена с помощью библиотеки plotly, для ее отображения на github все графики выгружены в формат png, к сожалению качество картинки оставляет желать лучшего и она не интерактивна, но для составления общего впечатления о  работе этого достаточно. Если проект долго грузится, пожалуйста, обновите страницу.

