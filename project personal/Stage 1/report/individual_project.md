---
## Front matter
title: "Отчёт по индивидуальному проекту"
subtitle: "Архитектура компьютеров и операционные системы"
author: "Вакутайпа Милдред"

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
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Быстрое развертывание сайта на GitHub Pages с помощью генератора статического html Hugo.

# Задание

- Установка программного обеспечения
- Установка темы
- Публикация сайта

# Выполнение лабораторной работы

## Установка программного обеспечения

Установливаю программу вручную с репозитория на Github:

![Установка Hugo](image/1.PNG){#fig:001 width=70%}

Распаковаю программу и копирую её в bin:

![Распаковка ](image/2.PNG){#fig:002 width=70%}

По шаблону Academic-cv создаю новый репозиторий blog:

![blog](image/4.PNG){#fig:003 width=70%}

Клонирую репозиторий, который содержит структуру сайта в каталог work/blog :

![Клонирование](image/5.PNG){#fig:004 width=70%}

Перехожу в этот же каталог и проверяю с помощью ls -l:

![Проверка](image/6.PNG){#fig:005 width=70%}

## Установка темы

Запускаю hugo:

![Запуск hugo](image/7.PNG){#fig:006 width=70%}

Запускаю программу с командой server, чтобы видеть сайт на локальный сервер:

![hugo server](image/8.PNG){#fig:007 width=70%}

![Сайт на локальном сервере](image/10.PNG){#fig:008 width=70%}

Создаю еще один репозиторий имя, которое является адресом сайта:

![новый репозиторий](image/11.PNG){#fig:009 width=70%}

Клонирую созданный репозиторий, который храняется у себя в каталог wakutaipa.github.io:

![Клонирование](image/12.PNG){#fig:0010 width=70%}

Создаю новую ветку с именем main:

![Новая ветка](image/13.PNG){#fig:0011 width=70%}

## Публикация сайта

Создаю пустой файл readme.md и отправляю на глобальный репозиторий:

![git push](image/14.PNG){#fig:0012 width=70%}

Комментирую public с помощью mc в .gitignore чтобы каталоги с таким названием не игнорировались:

![.gitignore](image/17.PNG){#fig:0013 width=70%}

Добавляю репозиторий к каталогу с помощью git submodule add:

![git submodule add](image/18.PNG){#fig:0014 width=70%}

Запускаю hugo, чтобы заполнить созданный каталог:

![Запуск hugo](image/19.PNG){#fig:0015 width=70%}

Провеяю подключение между созданным каталогом и wakutaipa.github.io:

![Проверка подключением](image/21.PNG){#fig:0016 width=70%}

Далее отправляю все файлы на github:

![Отправка файлы](image/22.PNG){#fig:0017 width=70%}

![Отправка файлы](image/23.PNG){#fig:0018 width=70%}

![wakutaipa.github.io](image/23.PNG){#fig:0019 width=70%}

# Выводы

При выполнении данной работы я научилась, как развмещать сайт на GitHub Pages с помощью генератора статического html Hugo.

# Список литературы{.unnumbered}

[Creating Hugo Site](https://yamadharma.github.io/ru/post/2022/04/12/creating-hugo-site/)
