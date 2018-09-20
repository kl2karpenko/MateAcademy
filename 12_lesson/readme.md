## Using SASS please create folowing CSS rules:

1. Create a file with variables:

```
backColor - #ffcccc;
buttonBackColor - #2a602d;
buttonBackActiveColor - #334432;
mainSize - 14px;
fontFamily - "Helvetica";
textColor - #333;
countBlocks - 5;
```
2. Create a button, height: 40px, with padding on the left and right. Add for it styles for active state, focus state and hover state. All of the state should be different from each other.
3. Create CSS rules for blocks, to make this list beutifull usign SASS syntax and **&** when creating styles. Every task should be on 1 line using next HTML:
```html
<div class="tasks__wrapper">
  <ul class="tasks__list">
    <li class="tasks__item">
      <span class="tasks__item-remove"></span>
      <span class="tasks__item-text">First task</span>
    </li>
    <li class="tasks__item">
      <span class="tasks__item-remove"></span>
      <span class="tasks__item-text">Second task</span>
    </li>
    <li class="tasks__item">
      <span class="tasks__item-remove"></span>
      <span class="tasks__item-text">Third task</span>
    </li>
  </ul>
</div>
```
4. Create the same **tasks__list** as in the previous task, but make every task item as a table cell, fit by 33% of the task wrapper and change a little bit styles for the list, here please create different file for this styles, and add common styles to 1 file, and use SASS templates here (eg: %[style-name] {})
5. Create a sass mixin for styling next HTML, rules for styling are: "every next .rules__item should have font-size bigger then previous on 1px, and it should have randow color"
```html
<div class="rules">
  <div class="rules__item">1 rule</div>
  <div class="rules__item">2 rule</div>
  <div class="rules__item">3 rule</div>
  <div class="rules__item">4 rule</div>
  <div class="rules__item">5 rule</div>
  <div class="rules__item">6 rule</div>
</div>
```
6. Create messenger as this one https://raw.githubusercontent.com/FLCreative/ng2-toastr/HEAD/toastr-examples.jpg?raw=true with 5 styles (success, error, info, warning and default) using SASS **maps** and **@each** directives. Every style has it's own styles for **background, color, text-color, icon status**
7. Using @for directive in SASS create a document with 20 stairs (eg: https://maxcdn.icons8.com/Share/google/s/stairs.png), where every stair bigger on 15px then previous one
8. Using SASS cycles (while or for) create a table with 15 rows, where every odd row will be blue, every even yellow, every 5 row: black and every 8 block - green.
9. Create buttons using Mapping and cycles (for or while) in SASS with 5 types: "success, warning, info, default and error" and each with different sizes: "small, iddle and big"

## Create a project using BEM technologies:

Create a login and registration https://nayvii.com/wp-content/uploads/2018/07/web-site-login-and-registration-form-free-psd-design-download-ux-tem-ui-inspiration-examples-studio-in-bootstrap-html-element-best-practices-css-672x622.jpg


