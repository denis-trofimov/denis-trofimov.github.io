---
title: Простые вопросы по Javascript для интервью
authors:
  - denis
type: blog
date: 2018-06-25T23:29:33+00:00
featured_image: WhatAboutAsynchronousCallbacks.png

categories:
  - learning
tags:
  - course
  - interview
  - javascript
  - learning
  - questions
---
В этом посте я рассказываю о некоторых основных вопросах и ответах на Javascript, которые я задал в ходе курса [**JavaScript LaunchPad**][1] **от** **[Simple Programmer.com.][2]**

В 2017 году я провел собеседование с тремя людьми на должность разработчика в компании, в которой работаю, ООО «Взор Системс».

Оказалось, что для подготовки к интервью со стороны интервьюера нужно приложить некоторые усилия. Если компания – не большой, а небольшой стартап, моя работа как интервьюера — придумывать вопросы и письменные тесты для проверки навыков и знаний кандидата. Однажды я искал типичные вопросы на собеседовании на должность разработчика C++.

Учитывая поле зрения интервьюера, я создал этот список вопросов, когда закончил первую **[JavaScript LaunchPad][1] **главу «**Контексты выполнения и лексические среды».**

<!--подробнее-->

## Контекст выполнения – создание и подъем

### Вопрос: Что этот код выдаёт на консоль?

```javascript
b();
console.log(a);
var a = 'Hello World!';
function b() {
  console.log('Called b!');
}
```

### Ответ:

```javascript
Called b!
Hello World!
```

## Функции, контекст и переменная среда

### Вопрос: Что этот код выдаёт на консоль?

```javascript
function b() {
  var myVar;
  console.log(myVar);
}
function a() {
  var myVar = 2;
  console.log(myVar);
  b();
}
var myVar = 1;
console.log(myVar);
a();
console.log(myVar);
```

### Ответ:

```javascript
1
2
1
1
```

## Цепочка прицелов

### Вопрос: Что этот код выдаёт на консоль?

```javascript
function a() {
  function b() {
    console.log(myVar);
  }
  b();
}
var myVar = 1;
a();
b();
```

### Ответ:

```javascript
1
Uncaught ReferenceError: b is not defined
``` 

## А как насчет асинхронных обратных вызовов

### Вопрос: Что этот код выдаёт на консоль?

```javascript
// long running function
function waitThreeSeconds() {
  var ms = 3000 + new Date().getTime();
  while (new Date() < ms){}
  console.log('finished function');
}
function clickHandler() {
  console.log('click event!');
}
// listen for the click event
document.addEventListener('click', clickHandler);
waitThreeSeconds();
console.log('finished execution');
```

### Ответ:

```javascript
finished function
finished execution
click event!
```

 [1]: https://simpleprogrammer.com/store/products/javascript-launchpad/?c=jslp70&utm_source=drip&utm_medium=email&utm_campaign=js-launchpad-sale&utm_content=js-launchpad-sale-email-2&__s=25hdpkywdqsodfst7mgj&utm_source=drip&utm_medium=email&utm_campaign=JavaScript+LaunchPad+Introduction&utm_content=Q%26A+about+JavaScript+LaunchPad
 [2]: https://simpleprogrammer.com/