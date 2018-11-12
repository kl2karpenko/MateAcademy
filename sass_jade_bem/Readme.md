# Practice Sass and Jade
You need to markup card from UI kit - https://zpl.io/Vx1d67k

## Tasks
### Level 0
  1. Download [zeplin](https://zeplin.io)
  2. Finish processing SASS and Jade using Gulp task
  
### Level 1
  1. Create file `main.scss` in the *src* folder
  2. Also create `_variables.scss` and `_mixins.scss` partials in the *src* folder. Import both of them into *main.scss* file
  3. Create directory *components* in the *src* folder 
    * 3.0 Define colors and texts for buttons in `_variables.scss`
    * 3.1. Create folder *button* inside components folder, create `_buttons.sass` which describe two types of buttons:
      
      - design https://zpl.io/2plAnjj
      - example of implementation - https://material.angular.io/components/button/overview
      - ripple effect 
        
        - css https://codepen.io/rudnitskih/pen/vQKvJa?editors=1100
        - js https://codepen.io/ayoisaiah/pen/GWwabJ
  
  4. Create `button.pug` in the *button* folder with mixin which desribe button
      - how to create jade mixin - https://codepen.io/rudnitskih/pen/GYVQxg
      - what is attribitues in pug - https://pugjs.org/language/mixins.html#mixin-attributes  
  5. Create `index.pug` file and add section with examples of your buttons - https://zpl.io/2plAnjj
      * 5.1 Don't forget add Roboto font (https://material-ui.com/getting-started/installation/)
  
### Level 2
  1. Create mixins which desribes different `box-shadows` - https://zpl.io/VYkEMgp (Create 5 mixins for each level of depth)
  2. Create folder `card` in `src`, and `card.pug` in this directory
  3. Create Card component using BEM notation
      * 3.1 Create `card` mixin which will just looks like required card with hardcoded texts
      * 3.2 Show Show example of card component in `index.pug`
  
  4. Split card implementation to different mixins support such usage:
```jade
  +card
    +card-header
      Card headline title

    +card-content
      Lorem ipsum dolor sit amet, doming noster at quo, nostrud lucilius rationibus ea duo.

    +card-footer({
      withDevider: true
    })
      +button({
        text: "DECLINE!"
      })
      +button({
        text: "ACCEPT"
        type: "flat"
        colored: true
      })
```
  5. Render two cards in `index.pug`
  
  
### Level 3
  1. Add mixins to add 3 dots in the end of line - https://gist.github.com/plapier/4954935, use it for title in the card
  2. Add mixins which describes breakpoints - https://css-tricks.com/approaches-media-queries-sass/#article-header-id-3
  3. Increate text in `x1.25` on tablet and `x1.33` on mobile in a card component
  

### Advanced tasks:
 1. Refactor mixins with `box-shadows` to one mixin which accept level of depth in argument   
 2. Add namespace to all classes
 3. Add documentation how to use your library - https://material-ui.com/getting-started/installation/
