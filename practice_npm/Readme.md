# Create your own Gulp config

## Tasks:
### First level:
  - install `nvm`
  - install `node`
  - install `npx`

### Second level:
  - create new project and init it as NPM package
  - disable generating package-lock.json - https://codeburst.io/disabling-package-lock-json-6be662f5b97d
  - in the folder `src` create one HTML file,
  - in the folder `src` create folder `css` with two CSS files
  - in the folder `src` create folder `images` with at least one image file
  - in the folder `src` create folder `fonts` with at least one font
  - use all css styles, images and fonts in your project
  - install Gulp locally(!!!) and create `gulpfile.js`

 
### Third level - create the following Gulp tasks:
  - copy all html files, fonts and images from `src` folder to `dist`
  - create task to clean dist folder on every run
  - concat all CSS files into one and put one css file into `dist` folder
  - run local webserver to serve dist folder
  - watch changes for every particular file type and run appropriate task
  - add `autoprefixer` task to your CSS files
  - describe all the main tasks in the `npm scripts` section
  - optimize images before saving them into `dist` folder
