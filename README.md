# NATOURS

Float layout - front-end project

Special scripts:

"scripts": {
"watch:sass": "node-sass sass/main.scss css/style.css -w",
"compile:sass": "node-sass sass/main.scss css/style.comp.css",
"concat:css": "concat -o css/style.concat.css css/ICONFONT/styles.css css/style.comp.css",
"prefix:css": "postcss --use autoprefixer -b 'last 10 versions' css/style.concat.css -o css/style.prefix.css",
"compress:css": "node-sass css/style.prefix.css css/style.css --output-style compressed",
"build:css": "npm-run-all compile:sass concat:css prefix:css compress:css"
},

npm run build:css
