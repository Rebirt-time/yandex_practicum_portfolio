<img src="mobile_brothers.png" width=200 align="right"/>

# Описание проекта - Изучение и анализ одноимённой мобильной игры в компании "Космические братья"

## Презентация проекта: [Космические братья](https://drive.google.com/file/d/1rOp9YTkxAIz7CmJvEJEIoS9PqY0Yf2PF/view?usp=share_link) 
## Дашборд проекта: [Космические братья](https://public.tableau.com/app/profile/shinelev.artem/viz/SpacebrothersArtem/Dashboard1?publish=yes)

В игре пользователи строят свою космическую программу и пытаются преуспеть в нелёгком деле колонизации галактики.

Основная монетизация игры — только планируется. Но предполагается, что в приложении будет происходить показ рекламы на экране с выбором типа объекта для постройки.

В датасете представлены данные по игре пользователей на первом уровне. Завершение первого уровня требует от игрока выполнения одного из двух условий:

- Победа над первым врагом
- Реализация проекта - разработка орбитальной сборки спутников

В датасете содержатся данные первых пользователей приложения — когорты пользователей, которые начали пользоваться приложением в период с 4 по 10 мая 2020 года, включительно.

Сформулируем модель монетизации игрового приложения

Многие игры зарабатывают с помощью рекламы. И все они сталкиваются с противоречием;

- Пользователь разозлится и уйдёт, если начать показывать ему рекламу раньше, чем игра его затянет.
- Но чем позже создатели игры включат рекламу, тем меньше они заработают.

Аналитик помогает бизнесу выбрать оптимальное время для запуска рекламы. Зная расходы на продвижение игры, он может рассчитать её окупаемость при разных сценариях 

Пока создатели игры планируют показывать её на экране выбором постройки. Поможем им не уйти в минус.



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
</div> 

## Задача:

Помочь не уйти в минус создателям игрового приложения при показе рекламы на экране выбора постройки

Сформировать модель монетизации игрового приложения:
- Общий доход > общего расхода 
- Расходы на рекламу должны быть меньше доходов

Нам предстоит изучить:
1.	откуда приходят пользователи,
2.	сколько стоит привлечение пользователей из различных рекламных каналов;
3.	сколько денег приносит каждый клиент,
4.  предоставить презентацию по проекту
5.  предоставить дашборд

## Данные:

Для анализа нам предоставлены три датасета в них содержится следующая информация:

- с игрой, содержит данные о событиях в игре, представленные пользователями на первом уровне.
- информация расходов на рекламу
- информация о пользователях, пришедших в приложение

**Структура сета с игрой:**

- event_datetime — время события;
- event — одно из трёх событий:
- building — объект построен,
- finished_stage_1 — первый уровень завершён,
- project — проект завершён;
- building_type — один из трёх типов здания:
- assembly_shop — сборочный цех,
- spaceport — космопорт,
- research_center — исследовательский центр;
- user_id — идентификатор пользователя;
- project_type — тип реализованного проекта;

**Структура сета с расходов на рекламу:**

- day - день, в который был совершен клик по объявлению
- source - источник трафика
- cost - стоимость кликов

**Структура сета с пользователями:**

- user_id - идентификатор пользователя
- source - источников, с которого пришёл пользователь, установивший приложение
