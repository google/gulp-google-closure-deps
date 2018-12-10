# gulp-google-closure-deps

This is a Gulp plugin for [Google Closure deps](https://github.com/luzhang/closure-library/tree/master/closure-deps).


## Install

Install via npm:

```
npm install gulp-google-closure-deps
```

To use the CLI below from any directory install the package globally:

```
npm install -g gulp-google-closure-deps
```


## Usage

```js
const closureDeps = require('gulp-google-closure-deps');

gulp.task('deps', function() {
  return gulp.src('./src/js/**/*.js')
    .pipe(closureDeps({'closurePath': './node_modules/google-closure-library/closure/goog'}))
    .pipe(rename('deps.js'))
    .pipe(gulp.dest('public'));
});
```




