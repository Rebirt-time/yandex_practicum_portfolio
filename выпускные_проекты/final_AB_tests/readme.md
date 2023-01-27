<img src="ab_test.png" width=200 align="right"/>

# Описание проекта - A/B-тестирование 

В нашем распоряжении есть датасет с действиями пользователей, техническое задание и несколько вспомогательных датасетов.


## Используемые технологии:
<div align="left">
<a href="https://www.python.org" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"/></a>
<a href="https://pandas.pydata.org" target="_blank"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</a>
<a href="https://jupyter.org" target="_blank"><img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Numpy-B0E0E6?style=for-the-badge&logo=Numpy&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Scipy-191970?style=for-the-badge&logo=Scipy&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Matplotlib-808080?style=for-the-badge&logo=CodeForces&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Datetime-FFFF00?style=for-the-badge&logo=Datetime&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Plotly-000000?style=for-the-badge&logo=Plotly&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Seaborn-047DA3?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Math-2F4F4F?style=for-the-badge&logo=Math&logoColor=white"/>
</a>
</div> 

## Задача:

На основе полученных данных исследовать результат:
- провести оценку результатов A/B-теста,
- оценить корректность проведения теста,
- проанализировать результаты теста.

Чтобы оценить корректность проведения теста, проверим:

- пересечение тестовой аудитории с конкурирующим тестом,
- совпадение теста и маркетинговых событий, другие проблемы временных границ теста.

**Производить исследование будем согласно тезническому заданию:**

- Название теста: `recommender_system_test`;
- группы: А — контрольная, B — новая платёжная воронка;
- дата запуска: 2020-12-07;
- дата остановки набора новых пользователей: 2020-12-21;
- дата остановки: 2021-01-04;
- аудитория: 15% новых пользователей из региона EU;
- назначение теста: тестирование изменений, связанных с внедрением улучшенной рекомендательной системы;
- ожидаемое количество участников теста: 6000.
- ожидаемый эффект: за 14 дней с момента регистрации пользователи покажут улучшение каждой метрики не менее, чем на 10%:
    - конверсии в просмотр карточек товаров — событие `product_page`,
    - просмотры корзины — `product_cart`,
    - покупки — `purchase`.

## Данные:

Для анализа нам предоставлены четыре датасета в них содержится следующая информация:

*календарь маркетинговых событий на 2020 год:*

- название маркетингового события;
- регионы, в которых будет проводиться рекламная кампания;
- дата начала кампании;
- дата завершения кампании.

*пользователи, зарегистрировавшиеся с 7 по 21 декабря 2020 года:*

- идентификатор пользователя;
- дата регистрации;
- регион пользователя;
- устройство, с которого происходила регистрация.

*действия новых пользователей в период с 7 декабря 2020 по 4 января 2021 года:*

- идентификатор пользователя;
- дата и время покупки;
- тип события;
- дополнительные данные о событии. Например, для покупок, purchase, в этом поле хранится стоимость покупки в долларах.

*таблица участников тестов:*

- идентификатор пользователя;
- название теста;
- группа пользователя.
