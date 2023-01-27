<img src="free_game.png" width=200 align="right"/>

# Описание проекта - Исследуем интернет-магазин "Стримчик" .Выявим определяющие успешность игры закономерности.

Мы работаем в интернет-магазине «Стримчик», который продаёт по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation). Нам нужно выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании.

Перед нами данные до 2016 года. Представим, что сейчас декабрь 2016 г., и мы планируем кампанию на 2017-й. Нужно отработать принцип работы с данными.

В наборе данных попадается аббревиатура ESRB (Entertainment Software Rating Board) — это ассоциация, определяющая возрастной рейтинг компьютерных игр. ESRB оценивает игровой контент и присваивает ему подходящую возрастную категорию, например, «Для взрослых», «Для детей младшего возраста» или «Для подростков».

## Используемые технологии
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
</div> 

## Задача

На основе изучения информации о пользователях, консолях и играх исследовать:
- популярность игровых платформ на определённом этапе
- выявить самые популярные игровые жанры 
- составить портреть пользователя каждого региона 
- влияние ESRB рэйтинга на продажу игр 
- одинаковы ли средние пользовательские рейтинги платформ Xbox One и PC?
- одинаковы ли средние пользовательские рейтинги жанров Action (англ. «действие», экшен-игры) и Sports (англ. «спортивные соревнования»)?


## Данные
Датасет содержит следующую информацию:

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
- Rating — рейтинг от организации ESRB (англ. Entertainment Software Rating Board). Эта ассоциация определяет рейтинг компьютерных игр и присваивает им подходящую возрастную категорию.
