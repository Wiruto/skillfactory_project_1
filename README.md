<center> <img src = https://raw.githubusercontent.com/AndreyRysistov/DatasetsForPandas/main/hh%20label.jpg alt="drawing" style="width:400px;"></center>

# <center> Анализ резюме из Head Hunter </center>


## Оглавление
1. [Описание проекта](#Описание-проекта)
2. [Описание данных](#Описание-данных)
3. [Зависимости](#Зависимости)
4. [Установка проекта](#Установка-проекта)
5. [Использование проекта](#Использование-проекта)
6. [Авторы](#Авторы)
7. [Выводы](Использование-проекта)

## Описание проекта
> Проблема компании HeadHunter залючается в том, что часть соискателей не указывает желаемую заработную плату, когда составляет своё резюме.
Это является помехой для рекомендательной системы HeadHunter, которая подбирает соискателям список наиболее подходящих вакансий, а работодателям — список наиболее подходящих специалистов.
Компания  хочет построить модель, которая бы автоматически определяла примерный уровень заработной платы, подходящей пользователю, исходя из информации, которую он указал о себе.

Задача проекта заключается в подготовке исходных данных для построения модели.

Основные этапы подготовки данных:
* Базовый анализ структуры данных;
* Преобразование данных;
* Разведовательный анализ данных;
* Очистка данных.



**Базовый анализ структуры данных** — знакомство с данными и исследования их структуры. Нам важно понять, как устроены признаки в данных, какой тип имеют данные в датасете, есть ли в признаках пропуски, какая статистикая информация по каждому признаку. Данный анализ помогает, в том числе, выявить признаки в которых данные представлены в неудобном для построения модели формате.

**Преобразование данных** — Выявленные в ходе базового анализа признаки преобразовываются к формату "пригодном" для дальшейго построения модели.
На этом этапе возможно создание новых признаков из существующих, преобразование типа данных, удаление не информативных признаков.

**Разведовательный анализ данных (исследование зависимостей данных)** —  Анализ, который предназначен для выявления связей между признаками, выявления закономерностей, определения распределений признаков, поиска аномалий и других дефектов данных.
На этом этапе используются инструменты визуализации данных для представления и анализа зависимостей различных признаков.

**Очистка данных** — процесс избавления от «мусора», который может помешать моделированию или исказить его результаты. Во многих задачах очистка данных — это самая главная часть этапа подготовки данных к построению модели, которая нередко занимает большую часть времени работы над задачей. В данном проекте в процессе проведения базового и разведовательного анализа выявляются признаки с пропусками и данные с анамальными и ошибочными значениями. Эти данные должны быть рассмотрены на предмет очистки из результирующего Data Frame.

**Данный проект** направлен на демонстрацию умения работы с библиотеками Pandas, Numpy, Plotly. Демострацию навыков работы с функциям, lambda-функциями; умения работать с условными операторами, циклическими операторами; умения анализировать большие базы данных с помощью упомянутых инструментов.

**О структуре проекта:**

* [plotly](https://github.com/Wiruto/skillfactory_project_1/tree/master/plotly) - папка с интерактивной графикой построенной с помощью библиотеки plotly;
* [project-1.ipynb](https://github.com/Wiruto/skillfactory_project_1/blob/9a05c33102ade96717aff5949afb9cae39d9e099/Project-1.ipynb) - jupyter-ноутбук, содержащий основной код проекта.


## Описание данных
В этом проекте используются база данных резюме, выгруженная с сайта поиска вакансий hh.ru.
Файл с базой резюме вы можете скачать [здесь](https://drive.google.com/file/d/1oMiFCZPO3AG9aIMUE3GpMJiWG5zYwVVZ/view?usp=share_link)

Исходный датасет представляет собой набор данных из таблицы с информацией которую о себе указали соискатели. Датасет содержит 12 признаков. 

Для преобразования одного из признаков, в проекте был необходим датасет с информацией о текущем курсе валют, которые встречатся в данных исходного датасета за период с 29.12.2017 по 05.12.2019. Скачать датасет вы можете [здесь](https://drive.google.com/file/d/1NzAUWZzEj6myuubjjS2Zgap9Nl8BQ6v9/view?usp=share_link)

## Используемые зависимости
* Python (3.9):
    * [numpy (1.24.1)](https://numpy.org)
    * [pandas (1.5.3)](https://pandas.pydata.org)
    * [plotly (5.13.0)](https://plotly.com)

## Установка проекта

```
git clone https://github.com/Wiruto/skillfactory_project_1.git

```

## Использование
Вся информация о работе представлена в jupyter-ноутбуке [project-1.ipynb](https://github.com/Wiruto/skillfactory_project_1/blob/9a05c33102ade96717aff5949afb9cae39d9e099/Project-1.ipynb).

## Авторы

* [Колобов Виктор Валерьевич](https://github.com/Wiruto)

## Выводы

1. В ходе базового анализа в исходном датасете были найдены не информативные признаки. Автор проекта создал новые признаки на их основе, выделив из таких признаков информативную часть. Часть признаков было удалено.
2. После разведовательного анализа данных в исходном датасете были выявлены выбросы и пропуски в данных. Они были удалены из датасета.
3. После подготовки данных, результирующий датасет содержит 23 признака и 44482 строки данных.