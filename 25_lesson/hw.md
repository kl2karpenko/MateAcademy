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

Создайте таблицу с 10 стороками и столбцами!
Напишите код, который выделит все ячейки в таблице по диагонали.
Вам нужно будет получить из таблицы table все диагональные td и выделить их, используя код:

```javascript
// в переменной td DOM-элемент для тега <td>
td.style.backgroundColor = 'red';

```

## 3 task

Напишите функцию createSpanInBlockByID(blockID) которая будет создавать элемент 'span' в блоке id=blockID 

P.S. Эта функция должна проверять наличие элемента в этом блоке, если он уже там есть второй раз она его добавлять не будет!

## 4 task

Создайте функцию createCloneNode(block) которая которая будет клонировать передаваемый ей элемент и добавять его в конец страницы! 

## 5 task

Создайте функцию addChildrenTo(block, count, type) которая будет создавать внутри block count количество детей типа type ( type это будет тип блока например 'span, ul, li, div' и т.д.  )

## 6 task

Напишите функцию replaceElBy(blockCurrent, blockToReplace) которая будет заменять blockCurrent на blockToReplace и выводить сообщение пользователю после успешного проведения операции!

## 7 task

Создайте элемент #test. По клику на него выведите название его тега.

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
