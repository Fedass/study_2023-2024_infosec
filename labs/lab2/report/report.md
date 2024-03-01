---
## Front matter
title: "Отчёт по лабораторной работе №2"
subtitle: "Дискреционное разграничение прав в Linux. Основные атрибуты"
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

Получение практических навыков работы в консоли с атрибутами файлов, закрепление теоретических основ дискреционного разграничени доступа в современных системах с открытым кодом на базе ОС Linux.
                                                                             

# Выполнение лабораторной работы


1. B установленной при выполнении предыдущей лабораторной работы
операционной системе создайте учётную запись пользователя guest (использую учётную запись администратора)
![image1](image/1.png)
2. Задайте пароль для пользователя guest (использую учётную запись ад-
министратора):
![image2](image/2.png)
3. Bойдите в систему от имени пользователя guest.
![image3](image/3.png)
4. Oпределите директорию, в которой вы находитесь, командой pwd. Срав-
ните её с приглашением командной строки. Определите, является ли она
вашей домашней директорией? Если нет, зайдите в домашнюю директо-
рию.
![image4](image/4.png)
5. Уточните имя вашего пользователя командой whoami.
![image5](image/5.png)
6. Уточните имя вашего пользователя, его группу, а также группы, куда вхо-
дит пользователь, командой id. Выведенные значения uid, gid и др. за-
помните. Сравните вывод id с выводом команды groups.
![image6](image/6.png)
7. Просмотрите файл /etc/passwd командой cat /etc/passwd.Найдите в нём свою учётную запись. Определите uid пользователя. Определите gid пользователя. Сравните найденные значения с полученными в предыдущих пунктах
![image7](image/7.png)
8. Oпределите существующие в системе директории командой ls -l /home/
Удалось ли вам получить список поддиректорий директории /home? Какие права установлены на директориях?
![image9](image/9.png)
9. Проверьте, какие расширенные атрибуты установлены на поддиректориях, находящихся в директории /home, командой:
lsattr /home. Удалось ли вам увидеть расширенные атрибуты директории? Удалось ли вам увидеть расширенные атрибуты директорий других пользователей?
![image10](image/10.png)
10. Создайте в домашней директории поддиректорию dir1 командой
mkdir dir1. Определите командами: ls -l и lsattr, какие права доступа и расширенные атрибуты были выставлены на директорию dir1.  Снимите с директории dir1 все атрибуты командой: chmod 000 dir1 и проверьте с её помощью правильность выполнения команды: ls -l.
![image11](image/11.png)
11. Попытайтесь создать в директории dir1 файл file1 командой: echo "test" > /home/guest/dir1/file1
Объясните, почему вы получили отказ в выполнении операции по созданию файла? Оцените, как сообщение об ошибке отразилось на создании файла? 
![image12](image/12.png)
12. Hа основании заполненной таблицы определите те или иные минимально необходимые права для выполнения операций внутри директории dir1, заполните табл. 2.2.
![image13](image/13.png)










# Выводы

В итоге научился использовать атрибуты в консоли линукс Rocky.

# Список литературы{.unnumbered}

::: {#refs}
:::
