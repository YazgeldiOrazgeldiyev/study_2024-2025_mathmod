---
## Front matter
title: "Лабораторная работа 4"
subtitle: "Математическое моделирование"
author: "Оразгелдиев Язгелди"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Реализовать математическую модель гармонического осциллятора

# Задание

Построить фазовый портрет гармонического осциллятора и решение уравнения гармонического осциллятора для следующих случаев

1. Колебания гармонического осциллятора без затуханий и без действий внешней силы x''+6x=0
2. Колебания гармонического осциллятора с затуханием и без действий внешней силы x''+6x'+6x=0
3. Колебания гармонического осциллятора с затуханием и под действием внешней силы x''+6x'+12x=sin(6t)

t = [0,60]
x0=0.6
y0=1.6

# Выполнение лабораторной работы

1. Построил модель колебания гармонического осциллятора без затуханий и без действий внешней силы на языке Julia

![код на языке Julia](image/1.jpg){#fig:001 width=70%}

![Решение уравнения гармонического осциллятора без затуханий и без действий внешней силы](image/2.jpg){#fig:002 width=70%}

![Фазовый портрет гармонического осциллятора без затуханий и без действий внешней силы](image/3.jpg){#fig:003 width=70%}

Построил ту же модель на языке OpenModelica

![код на языке OpenModelica](image/4.jpg){#fig:004 width=70%}

![Решение уравнения гармонического осциллятора без затуханий и без действий внешней силы](image/5.jpg){#fig:005 width=70%}

![Фазовый портрет гармонического осциллятора без затуханий и без действий внешней силы](image/6.jpg){#fig:006 width=70%}

2. Построил модель колебания гармонического осциллятора с затуханием и без действий внешней силы на языке Julia

![код на языке Julia](image/7.jpg){#fig:007 width=70%}

![Фазовый портрет гармонического осциллятора с затуханием и без действий внешней силы](image/8.jpg){#fig:008 width=70%}

Построил ту же модель на языке OpenModelica

![код на языке OpenModelica](image/9.jpg){#fig:009 width=70%}

![Решение уравнения гармонического осциллятора с затуханием и без действий внешней силы](image/10.jpg){#fig:010 width=70%}

![Фазовый портрет гармонического осциллятора с затуханием и без действий внешней силы](image/11.jpg){#fig:011 width=70%}

3. Построил модель колебания гармонического осциллятора с затуханием и под действием внешней силы на языке Julia

![Решение уравнения гармонического осциллятора с затуханием и без действий внешней силы](image/12.jpg){#fig:012 width=70%}

![Фазовый портрет гармонического осциллятора с затуханием и без действий внешней силы](image/13.jpg){#fig:013 width=70%}

Построил модель колебания гармонического осциллятора с затуханием и под действием внешней силы на языке OpenModelica

![код на языке OpenModelica](image/14.jpg){#fig:014 width=70%}

![Решение уравнения гармонического осциллятора с затуханием и под действием внешней силы](image/15.jpg){#fig:015 width=70%}

![Фазовый портрет гармонического осциллятора с затуханием и под действием внешней силы](image/16.jpg){#fig:016 width=70%}


# Выводы

Я реализовал математическую модель гармонического осциллятора
