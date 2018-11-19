# Practice Sass and Jade
You need to markup card from UI kit - https://zpl.io/Vx1d67k

## Tasks
### Level 0
  1. Download [zeplin](https://zeplin.io)
  2. Finish processing SASS and Jade using Gulp task
  
### Level 1
  1. Create file `main.scss` in the *src* folder
  2. Also create `_variables.scss`, `_mixins.scss`and `_examples.scss` partials in the *src* folder. Import all of them into `main.scss` file
  3. Create directory *components* in the *src* folder 
      * 3.0 Define colors and texts for buttons in `_variables.scss`
      * 3.1. Сreate `_button.scss` which describe two types of buttons:
        - [design](https://zpl.io/2plAnjj)
        - [example of implementation](https://material.angular.io/components/button/overview)
        - ripple effect:
            * [css](https://codepen.io/rudnitskih/pen/vQKvJa?editors=1100)
            * [js](https://codepen.io/ayoisaiah/pen/GWwabJ)
  4. Create directory `src/examples/buttons.pug`
  5. Add example of your buttons to `buttons.pug`.
```
button.button Button
button.button.button_colored(href="//google.com") Colored

```
  6. Create `index.pug` and include `buttons.pug` into it
      * 6.1 Don't forget add Roboto font (https://material-ui.com/getting-started/installation/)
  
### Level 2
  1. Create mixins which desribes different `box-shadows` - https://zpl.io/VYkEMgp (Create 5 mixins for each level of depth)
  2. Create file `src/examples/box-shadows.pug` in describe examples of mixin usage in this file. Styles like `margins`, sizes of `div`s - describe them in `_examples.scss`
  3. Include `box-shadows.pug` into `index.pug`
  
### Level 3
  1. Create `src/examples/cards.pug` and markup standard card. 
  2. Create `components/_card.scss` and describe styles for it.
  3. Include `cards.pug` into `index.pug`.
  4. Also describe `simple` and `with-image` modifications. Describe `margins` beetween elements in  `_examples.scss`. Hint: use https://unsplash.com/ to find an example of image.
```
.card
  .card__title Card headline title
  .card__description Lorem ipsum dolor sit amet, doming noster at quo, nostrud lucilius rationibus ea duo. Vim no mucius dolores. No bonorum voluptatum vis, has iudicabit consectetuer ne. Nullam sensibus vim id, et quo graeci perpetua.
  .card__footer
    button.button.card__button MORE INFO…
    button.button.card__button.card__button_pulled DECLINE
    button.card__button.button.button-colore ACCEPT
```
### Level 4
  1. Add mixins which describes breakpoints - https://css-tricks.com/approaches-media-queries-sass/#article-header-id-3
  2. Increase text in `x1.25` on tablet and `x1.33` on mobile in a card component
  3. Refactor mixins with `box-shadows` to one mixin which accept level of depth in argument   
  4. Add namespace to all classes
