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
  5. Add example of your buttons to `button.pug`.
  5. Create `index.pug` and include `buttons.pug` into it
      * 5.1 Don't forget add Roboto font (https://material-ui.com/getting-started/installation/)
  
### Level 2
  1. Create mixins which desribes different `box-shadows` - https://zpl.io/VYkEMgp (Create 5 mixins for each level of depth)
  2. Create file `src/examples/box-shadows.pug` in describe examples of mixin usage in this file. Styles like `margins`, sizes of `div`s - describe them in `_examples.scss`
  3. Include `box-shadows.pug` into `index.pug`
  
### Level 3
  1. Create `components/_card.scss` and describe styles for it.
  2. Create `src/examples/cards.pug` and markup simple, standard and with-image cards. Describe `margins` beetween elements in  `_examples.scss`. Hint: use https://unsplash.com/ to find an example of image.
  3. Include `cards.pug` into `index.pug`.
  
### Level 4
  1. Add mixins to add 3 dots in the end of line - https://gist.github.com/plapier/4954935, use it for title in the card
  2. Add mixins which describes breakpoints - https://css-tricks.com/approaches-media-queries-sass/#article-header-id-3
  3. Increase text in `x1.25` on tablet and `x1.33` on mobile in a card component

### Level 5
 1. Refactor mixins with `box-shadows` to one mixin which accept level of depth in argument   
 2. Add namespace to all classes
