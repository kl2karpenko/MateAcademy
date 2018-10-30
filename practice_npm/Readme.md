# Create your own Gulp config

## Tasks:
### First level:
  - install `nvm`
  - install `node`
  - install `npx`

### Second level:
  - create new project and init it as NPM package
  - disable generating package-lock.json - https://codeburst.io/disabling-package-lock-json-6be662f5b97d
  - in the folder `src` create one HTML file
  - in the folder `src` create folder `css` with two CSS files
  - in the folder `src` create folder `images` with at least one image file
  - in the folder `src` create folder `fonts` with at least one font
  - use all css styles, images and fonts in your project
  - install Gulp locally(!!!) and create `gulpfile.js`

 
### Third level - create the following Gulp tasks:
  You can chose any gulp plugin which you will find, I provided the most popular plugins which I know.
  - copy all html files, fonts and images from `src` folder to `dist` (https://gulpjs.com/docs/en/api/src)
  - create task to clean dist folder on every run (e.g. https://www.npmjs.com/package/gulp-clean)
  - concat all CSS files into one and put one css file into `dist` folder (e.g. https://www.npmjs.com/package/gulp-concat)
  - run local webserver to serve dist folder (e.g. https://browsersync.io/docs/gulp) 
  - watch changes for every particular file type and run appropriate task (e.g. https://browsersync.io/docs/gulp#gulp-reload)
  - add `autoprefixer` task to your CSS files (e.g. https://www.npmjs.com/package/gulp-autoprefixer)
  - describe all the main tasks in the `npm scripts` section (e.g. https://stackoverflow.com/questions/27078245/automatic-run-gulp-tasks-via-npm)
  - optimize images before saving them into `dist` folder (e.g. https://www.npmjs.com/package/gulp-imagemin)
