---
## Front matter
title: "Отчёта по 5-му этапу индвидуального проекта"
subtitle: "по предмету 'Научное программирование'"
author: "Кирилл Валерьевич Дидусь"

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

Создания контента для персонализации шаблона сайта для научной коммуникации.

# Задание

- Добавить возможность просмотра контента на 2 языках.

# Теоретическое введение

Личный блог является важным инструментов в научной коммуникации. Он позволяет получить доступ к научным работам, связаться с автором и получить общее впечатление о нем. 

Для создания блога воспользуемся следующими инструментами:
- github
- github pages в качестве хостинга
- hugo (программа с шаблонами для быстрого создания сайтов)
- Wowchemy (подборка  тем для hugo)

# Выполнение лабораторной работы

1. Найдем папку /content и скопируем содержимое в подпапки с названием нужного языка. Используем /en для английского, как языка по-умолчанию, и /ru для поддержки русского языкаа.

2. Внесем необходимые изменения в конфиг-файл languages.yaml

3. Добавим перевод, где не сработал автоматический перевод элементов сайта. Затем переведем текст статей и отчетов в постах.

4. Выполним коммит изменений в соотвествующие репозитории и запустим сайт командой hugo. Затем проверим работоспособность сайта. Добавилась кнопка смены языка в шапке сайта. Все работает!

# Выводы

В результате работы мы имеем персонализированный шаблон сайта на github pages с поддержкой двух языков. На этом работа с сайтом в рамках индивидуального проекта завершается. Я планирую продолжать улучшать сайт и использать его в качестве визитки для научной коммуникации.

# Список литературы{.unnumbered}

- ТУИС РУДН
- HUGO
- WOWCHEMY
::: {#refs}
:::
