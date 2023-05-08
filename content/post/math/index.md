---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Научные языки программирования"
subtitle: "Один и тот же язык - два подхода"
summary: "Один и тот же язык - два подхода"
authors: []
tags: []
categories: []
date: 2023-04-25T20:10:53+03:00
lastmod: 2023-04-25T20:10:53+03:00
featured: false
draft: false


# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''
  focal_point: ''
  placement: 
  preview_only: false
  
authors:
  - admin

tags:
  - education
  - программирование

categories:
  - Demo
  
---
# Язык научного программирования - Scientific programming language

В компьютерном программировании , научный язык программирования может относиться к двум степеням той же концепции.

В широком смысле научный язык программирования - это язык программирования, который широко используется в вычислительной науке и вычислительной математике .

В этом смысле C / C ++ и Python можно рассматривать как языки научного программирования. В более строгом смысле научный язык программирования - это язык, который разработан и оптимизирован для использования математических формул и матриц . Такие языки характеризуются не только наличием библиотек, выполняющих математические или научные функции, но и синтаксисом самого языка. Например, ни C ++, ни Python не имеют встроенных типов матриц или функций для матричной арифметики (сложение, умножение и т. Д.); вместо этого эта функция доступна через стандартные библиотеки. Научные языки программирования в сильном смысле включают ALGOL , APL , Fortran , J , Юлю , Maple , MATLAB и R . 

Языки научного программирования не следует путать с научным языком в целом, который свободно относится к более высоким стандартам точности, правильности и краткости, ожидаемым от практикующих научный метод . 

# Примеры 

## Линейная алгебра

Языки научного программирования предоставляют возможности для работы с линейной алгеброй . Например, следующая программа Julia решает систему линейных уравнений :

A = rand(20, 20) # A is a 20x20 matrix

b = rand(20) # b is a 20-element vector 

x = A\b # x is the solution to A*x = b 

Работа с большими векторами и матрицами - ключевая особенность этих языков, поскольку линейная алгебра закладывает основу математической оптимизации , которая, в свою очередь, позволяет использовать основные приложения, такие как глубокое обучение . 

## Математическая оптимизация 

В научном языке программирования мы можем вычислять оптимум функции с синтаксисом, близким к математическому языку. Например, следующий код Джулии находит минимум полинома . 

using Optim 

P(x,y) = x^2 - 3x*y + 5y^2 - 7y + 3 

z₀ = [ 0.0 

0.0 ] # starting point for optimization algorithm o

ptimize(z -> P(z...), z₀, Newton(); 

autodiff = :forward)

В этом примере используется метод минимизации Ньютона . Современные языки научного программирования будут использовать автоматическое дифференцирование для вычисления градиентов и гессианов функции, заданной в качестве входных данных; ср. дифференцируемое программирование . Здесь для этой задачи выбрана автоматическая прямая дифференциация. Старые языки научного программирования, такие как почтенный Фортран, потребовали бы от программиста передать рядом с функцией, которая должна быть оптимизирована, функцию, которая вычисляет градиент, и функцию, которая вычисляет гессиан. 

Чем больше знаний о функции, которую необходимо минимизировать, тем больше можно использовать более эффективные алгоритмы. Например, выпуклая оптимизация обеспечивает более быстрые вычисления, когда функция является выпуклой, квадратичное программирование обеспечивает более быстрые вычисления, когда функция не более чем квадратична по своим переменным, и линейное программирование, когда функция максимально линейна. 