<img src="start_up.png" width=200 align="right"/>

# Описание проекта - Анализ стартапа пользователей мобильного приложения, который продаёт продукты питания. Изучение воронки продаж. Исследование результатов A/A/B эсперимента.

Я работаю в стартапе, который продаёт продукты питания. Нужно разобраться, как ведут себя пользователи нашего мобильного приложения.

Изучим воронку продаж. Узнаем, как пользователи доходят до покупки. Сколько пользователей доходит до покупки, а сколько — «застревает» на предыдущих шагах? На каких именно?

После этого исследуем результаты A/A/B-эксперимента. Дизайнеры захотели поменять шрифты во всём приложении, а менеджеры испугались, что пользователям будет непривычно. Договорились принять решение по результатам A/A/B-теста. Пользователей разбили на 3 группы: 2 контрольные со старыми шрифтами и одну экспериментальную — с новыми. Выясним, какой шрифт лучше.

Создание двух групп A вместо одной имеет определённые преимущества. Если две контрольные группы окажутся равны, мы можете быть уверены в точности проведенного тестирования. Если же между значениями A и A будут существенные различия, это поможет обнаружить факторы, которые привели к искажению результатов. Сравнение контрольных групп также помогает понять, сколько времени и данных потребуется для дальнейших тестов.

В случае общей аналитики и A/A/B-эксперимента работаем с одними и теми же данными. Исследуют качество работы приложения по общим данным, не учитывая принадлежность пользователей к экспериментам.


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
<a href=# target="_blank"><img src="https://img.shields.io/badge/Math-2F4F4F?style=for-the-badge&logo=Math&logoColor=white"/>
</a>
</div> 

## Задача:

На основе изученной информации, по пользователям, покупкам проанализируем:

- Как пользователи доходят до покупки?
- Сколько пользователей доходит до покупки, сколько «застревает» на предыдущих шагах и на каких?
- Исследуем результаты A/A/B экспериментаю.
- Выясним какой шрифт лучше после изменения дизайна.

## Данные:
В датасете содержится следующая информация:

Каждая запись в логе — это действие пользователя, или событие:
- EventName — название события;
- DeviceIDHash — уникальный идентификатор пользователя;
- EventTimestamp — время события;
- ExpId — номер эксперимента: 246 и 247 — контрольные группы, а 248 — экспериментальная.
