## 1 task

Here is a sample html file with a submit button. Write a JavaScript function to get the value of the href, hreflang, rel, target, and type attributes of the specified link.

```javascript
<!DOCTYPE html>  
<html>
  <head>  
    <meta charset=utf-8 />  
  </head>  
  <body>  
    <p>
      <a id="w3r" type="text/html" hreflang="en-us" rel="nofollow" target="_self" href="http://www.w3resource.com/">w3resource</a>
    </p>  
    <button onclick="getAttributes()">Click here to get  attributes value</button>  
  </body>
</html> 
```

## 2 task

Создайте input в который запретите водить некоторые символы (a, b, c, d, e). Любые другие символы должны вводится.

## 3 task

Напишите функцию createSpanInBlockByID(blockID) которая будет создавать элемент 'span' в блоке id=blockID 

P.S. Эта функция должна проверять наличие элемента в этом блоке, если он уже там есть второй раз она его добавлять не будет!

## 4 task

Дан инпут. При введени в него числа он должен отделять тройки чисел пробелами (по мере ввода).

## 5 task

Создайте функцию addChildrenTo(block, count, type) которая будет создавать внутри block count количество детей типа type ( type это будет тип блока например 'span, ul, li, div' и т.д.  )

## 6 task

Напишите функцию replaceElBy(blockCurrent, blockToReplace) которая будет заменять blockCurrent на blockToReplace и выводить сообщение пользователю после успешного проведения операции!

## 7 task

Дана таблица произвольного размера. По нажатию на ячейку таблицы эта ячейка красится красным фоном ("активируется"). Сделайте так, чтобы, если активировано 5 ячеек подряд по горизонтали или по вертикали, таблица блокировалась (то есть нельзя больше будет активировать ячейки) и выводилось сообщение "завершение активаций".

P.S. Хитрый прием с копировать и вставить из буфера обмена тоже нужно отловить, равно как и другие обходные пути.

## 8 task

Create function testNum() that will take 1 param: phone number string and define whether it have more than 8 symbols, 
contain only numbers (no slashes and spaces, if have replace them to empty string).

After that create an html page with input field and button, where user will write his/her phone number, 
after user press enter button on the right your function testNum() will check the phone number he enters 
and return to user ok (create span under the input field (color of text must be green)) - if pattern match, 
or error (the same create span with "error" text under (color of text must be red));

After 4 seconds delete the span and the input field should be empty again an the user can try again later.

```javascript
setTimeout(function () {
 // тут пишем наш код который будет выплняться через 4 секунды
}, 4000);
```

## 9 task

Покрасьте все буквы текста в заданном элементе в разные случайные цвета. Список цветов должен хранится в массиве.
Две соседние буквы не должны иметь одинаковый цвет.

## 10 task

Дан инпут. В него разрешено вводить N символов. При введение текста справа появляется счетчик такого типа - "Осталось ввести 10 символов". После того, как предел достигнут - текст все равно разрешено вводить, только надпись будет типа "Лимит превышен на 10 символов". Вместо 10-ти, конечно же, нужное число.

## 11 task

Write a JavaScript function to add rows to a table.

```javascript
<!DOCTYPE html>  
<html>
    <head>
        <meta charset=utf-8 />  
        <title>Insert row in a table - w3resource</title>  
    </head>
    <body>  
        <table id="sampleTable" border="1">  
        <tr><td>Row1 cell1</td>  
        <td>Row1 cell2</td></tr>  
        <tr><td>Row2 cell1</td>  
        <td>Row2 cell2</td></tr>  
        </table>
        
        <input type="button" onclick="insert_Row()" value="Insert row">   
    </body>
</html>  
```
