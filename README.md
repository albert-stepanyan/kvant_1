# Распознавание шрифтов 

## Описание проекта

Задача - распознавание шрифтов.

Цель - создание утилиты, которая принимает на вход изображение с текстом и распознает шрифт текста.

В папке fonts лежат шрифты для латинского алфавита. Шрифты были подобраны так, чтобы между ними было достаточно много различий.
Необходимо:

1.  Сгенерировать обучающую и тестовую выборки на основании шрифтов с помощью ЯП Python. 
    Можно использовать открытые библиотеки для генерации выборок. 
    В выборке должны присутствовать изображения всех шрифтов.
    Тексты должны быть на английском языке, тематика может быть любой (хоть случайная строка)
2.  Реализовать небольшое приложение для распознавания шрифтов

Приложение состоит из двух частей: модуль для обучения нейросети и модуль распознавания.

Модуль обучения:
1.  Содержит код нейросети
2.  Принимает на вход обучающую и тестовую выборки
3.  Обучает нейросеть, логгирует значения функции ошибки на обучающей и тестовой выборке. Логгировать можно любым образом (даже в txt или csv), главное чтобы
    можно было прочитать файл и отрисовать графики
4.  Оценивает основные метрики классификации, 
5.  Отрисовывает кривые обучающей и тестовой ошибок

Модуль обучения может быть либо консольным приложением, либо Jupyter-ноутбуком

Модуль распознавания является консольным приложением и принимает на вход путь до чекпойнта модели 
(или других служебных файлов) и возвращает название самого вероятного шрифта и его вероятность в консоль.

Для реализации используйте либо виртуальную среду virtualenv, либо Docker (желательно) для избежания конфликтов версий библиотек.

## План работы

1. Проведем подоготовку данных и создадим выборку изображений шрифтов.
2. Обучим нейронную сеть и рассчитаем её качество.
3. Создадим модуль распознавания шрифта.

## Результат работы в HTML

[Часть 1](https://raw.githack.com/albert-stepanyan/font_recognition/main/font_recognition_1.html)
[Часть 2](https://raw.githack.com/albert-stepanyan/font_recognition/main/font_recognition_2.html)
[Часть 3](https://raw.githack.com/albert-stepanyan/font_recognition/main/font_recognition_3.html)

## Работа выполнена с использованием

Python 3.11.7   
Pip 24.0    
Файл requirements.txt прилагается   
Файл fonts_sample.csv с перечнем используемых 15 шрифтов прилагается
