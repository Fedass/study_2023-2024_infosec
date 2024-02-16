---
## Front matter
title: "Отчет по лабораторной работе №1"
subtitle: "Установка и конфигурация операционной системы на виртуальную машину"
author: "Городянский Фёдор Николаевич"

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

Целью данной работы является приобретение практических навыков
установки операционной системы на виртуальную машину, настройки ми-
нимально необходимых для дальнейшей работы сервисов.

# Задание

Установка rocky и вывод информации в терминале. 


# Выполнение лабораторной работы

1. Создал новую виртаульную машину.
![im1](image/1.png){#fig:001 width=70%}
2. Указал имя виртуальной машины, тип
операционной системы — Linux, RedHat (64-bit), объем и тип диска, 
формат хранения,  имя и размер хранения.
![объем диска](image/2.png){#fig:002 width=70%}
![жесткий диска](image/3.png){#fig:003 width=70%}
![тип](image/4.png){#fig:004 width=70%}
![формат хранения](image/5.png){#fig:005 width=70%}
![имя и размер файла](image/6.png){#fig:006 width=70%}
3. Настройка rocky.
![im7](image/7.png){#fig:007 width=70%}
4. Выбор языка.
![выбор языка](image/8.png){#fig:008 width=70%}
5. Выбор загрузочного пространства.
![загрузка](image/9.png){#fig:009 width=70%}
6. Настройка пароля и логина.
![личные данные](image/10.png){#fig:010 width=70%}
7. Конец настройки.
![конец загрузки](image/11.png){#fig:011 width=70%}
![Роки!](image/12.png){#fig:012 width=70%}
8. Вывод общей информации.
![работа в терминале](image/13.png){#fig:013 width=70%}

 
# Выводы

В результате работы я настроил дистрибутив rocky и вывел базовую информацию в терминале.

