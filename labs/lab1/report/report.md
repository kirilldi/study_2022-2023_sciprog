---
## Front matter
title: "Отчёт по лабораторной работе 1"
subtitle: "по предмету: научное программирование "
author: "Дидусь Кирилл Валерьевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Подготовка рабочего пространства. Инициализация GIT и настройка GitHub.

# Задание

– Создать базовую конфигурацию для работы с git. 
– Создать ключ SSH.
– Создать ключ PGP.
– Настроить подписи git.
– Зарегистрироваться на Github.
– Создать локальный каталог для выполнения заданий по предмету.

# Выполнение лабораторной работы

Зарегистровался на сайте GitHub. Создал SSH ключ и ввел на сайте GitHub. Установил 'gh', прошел авторизацию и скопировал шаблон репозитория на свое устройство. Добавил необходимые файлы и выполнил команды 'git add .' и 'git push' для загрузки на github.
 
Таким образом был настроен и сконфигурирован рабочий репозиторий для выполнения лабораторных работ (рис. [-@fig:001]).

![Репозиторий проекта на github](image/1.png){ #fig:001 width=70% }

# Выводы

Результат выполнения работы настроенный рабочий репозиторий для выполнения лабораторных работ, с установленным ключом идентфикации ssh. В ходе работы освежил навыки работы с git
