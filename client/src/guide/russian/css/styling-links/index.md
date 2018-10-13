---
title: Styling Links
localeTitle: Ссылки для стилизации
---
## Ссылки для стилизации

Ссылки могут быть созданы с любым свойством CSS, таким как `color` , `font-family` , `font-size` и `padding` . Вот простой пример:

```css
a { 
    color: hotpink; 
 } 
```

## Кроме того, ссылки могут быть оформлены по-разному в зависимости от того, в каком состоянии они находятся.

В ссылках также есть 4 состояния, и многие программисты создают разные состояния по-разному. Четыре государства:

*   `a:link` : незатронутая, незакрепленная ссылка
*   `a:visited` : посещенная, кликнутая ссылка
*   `a:hover` : ссылка, когда мышь пользователя находится над ней
*   `a:active` : ссылка при нажатии

Свойство `<a href="">` отвечает за создание URL-адресов и может быть изменено с использованием нескольких свойств стилизации CSS, хотя по умолчанию у него несколько:

1.  подчеркивание
2.  Синий цвет

Вы можете изменить их, добавив изменения свойств `color` и `text-decoration` .

```css
   color: black; 
   text-decoration: none; 
```

Вы также можете создать ссылку на основе взаимодействия, используя эти свойства, также известные как состояния ссылок:

*   a: link - нормальная, незаметная ссылка
*   a: visited - ссылка, которую пользователь посетил
*   a: hover - ссылка, когда пользователь мыши над ней
*   a: active - ссылка в момент ее нажатия

Вот пример CSS с использованием четырех состояний:

```css
a:link { color: red; } 
 a:visited { color: blue; } 
 a:hover { color: green; } 
 a:active { color: blue; } 
```

**Обратите внимание,** что существуют некоторые _правила упорядочения,_ когда вы устанавливаете стиль для состояний ссылок.

*   `a:hover` ДОЛЖЕН прибыть после `a:link` и `a:visited`
    
*   `a:active` ДОЛЖЕН прийти после `a:hover`
    
    a: link - нормальная, незаметная ссылка a: visited - ссылка, которую пользователь посетил a: hover - ссылка, когда пользователь мыши над ней a: active - ссылка в момент ее нажатия
    

```css
/* unvisited link */ 
 a:link { 
    color: red; 
 } 
 
 /* visited link */ 
 a:visited { 
    color: green; 
 } 
 
 /* mouse over link */ 
 a:hover { 
    color: hotpink; 
 } 
 
 /* selected link */ 
 a:active { 
    color: blue; 
 } 

```