---
## Front matter
title: "Отчёта по 1-му этапу индвидуального проекта"
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

Размещение на Github pages заготовки для персонального сайта для научной коммуникации.

# Задание

- Установить необходимое программное обеспечение.
- Скачать шаблон темы сайта.
- Разместить его на хостинге git.
- Установить параметр для URLs сайта.
- Разместить заготовку сайта на Github pages.

# Теоретическое введение

Личный блог является важным инструментов в научной коммуникации. Он позволяет получить доступ к научным работам, связаться с автором и получить общее впечатление о нем. 

Для создания блога воспользуемся следующими инструментами:
- github
- github pages в качестве хостинга
- hugo (программа с шаблонами для быстрого создания сайтов)
- Wowchemy (подборка  тем для hugo)

# Выполнение лабораторной работы

1. Создадим 2 репозитория: 
- blog (клон из репозитория с академической темой wowchemy)
- kirillidi.github.io (репозитория для статичных файлов сайта, будущая страница сайта) (рис. [-@fig:001])

![Новые репозитории](image/1.png){ #fig:001 width=70% }

2. Клонируем репозиторий blog в каталог /blog и запустим локальный сервер hugo командой **hugo server** (рис. [-@fig:002]). 

![Клонированный репозитории](image/2.png){ #fig:002 width=70% }

3. Добавим подмодуль public в репозиторий blog. Перед этим обязательно добавим commit в репозиторий kirillidi.github.io, для избежания ошибок (рис. [-@fig:003]). 

![Создание подмодуля public](image/3.png){ #fig:003 width=70% }

4. Изменим baseURL в файле config.yaml на kirilldi.github.io (рис. [-@fig:004]).

![config.yaml](image/4.png){ #fig:004 width=70% }

5. Выполним коммит изменений в соотвествующие репозитории и запустим сайт командой hugo. Затем проверим работоспособность сайта. Все работает! (рис. [-@fig:005]).

![сайт на гитхаб пейджес](image/5.png){ #fig:005 width=70% }

# Выводы

В результате работы мы имеем шаблон сайта на github pages. В дальнейшем мы будем его редактировать.

# Список литературы{.unnumbered}

- ТУИС РУДН
- HUGO
::: {#refs}
:::
