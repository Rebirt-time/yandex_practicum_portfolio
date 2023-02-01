<img src="study.png" width=200 align="right"/>

# Описание проекта - Исследуем развлекательное приложения Procrastinate Pro+. Выясним, почему последние несколько месяцев компания терпит убытки.

Мы — маркетинговый аналитик развлекательного приложения Procrastinate Pro+. Несмотря на огромные вложения в рекламу, последние несколько месяцев компания терпит убытки. Ваша задача — разобраться в причинах и помочь компании выйти в плюс.
    Есть данные о пользователях, привлечённых с 1 мая по 27 октября 2019 года:
    •	лог сервера с данными об их посещениях,
    •	выгрузка их покупок за этот период,
    •	рекламные расходы.
    Вам предстоит изучить:
    •	откуда приходят пользователи и какими устройствами они пользуются,
    •	сколько стоит привлечение пользователей из различных рекламных каналов;
    •	сколько денег приносит каждый клиент,
    •	когда расходы на привлечение клиента окупаются,
    •	какие факторы мешают привлечению клиентов.


## Используемые технологии
<div align="left">
<a href="https://www.python.org" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"/></a>
<a href="https://pandas.pydata.org" target="_blank"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</a>
<a href="https://jupyter.org" target="_blank"><img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Numpy-B0E0E6?style=for-the-badge&logo=Numpy&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Matplotlib-808080?style=for-the-badge&logo=CodeForces&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Seaborn-047DA3?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Datetime-FFFF00?style=for-the-badge&logo=Datetime&logoColor=white"/>
</a>
</div> 

## Задача

На основе изучения информации о пользователях, расходов на рекламу и информации о заказах выяснить:

- откуда приходят пользователи и какими устройствами они пользуются
- сколько стоит привлечение пользователей из различных рекламных каналов
- сколько денег приносит каждый клиент
- когда расходы на привлечение клиента окупаются
- какие факторы мешают привлечению клиентов
- Почему последние месяцы компания приложения Procrastinate Pro+ терпит убытки.


## Данные
В датасетах содержится следующая информация:

Структура visits_info_short.csv:
- User Id — уникальный идентификатор пользователя,
- Region — страна пользователя,
- Device — тип устройства пользователя,
- Channel — идентификатор источника перехода,
- Session Start — дата и время начала сессии,
- Session End — дата и время окончания сессии.

Структура orders_info_short.csv:
- User Id — уникальный идентификатор пользователя,
- Event Dt — дата и время покупки,
- Revenue — сумма заказа.

Структура costs_info_short.csv:
- dt — дата проведения рекламной кампании,
- Channel — идентификатор рекламного источника,
- costs — расходы на эту кампанию.
