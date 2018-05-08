# gulp-json2pot

## Information

| Package     | gulp-json2pot                                          |
| ----------- | ---------------------------------------------------- |
| Description | Gulp wrapper for [json2pot](https://github.com/diosney/json2pot). Generate pot files from JSON keyed translation files via Gulp. |


## Install

```
$ npm install --save-dev gulp-json2pot
```


## Example usage with [Gulp](http://github.com/gulpjs/gulp)

```js
var gulp = require('gulp');
var json2pot = require('gulp-json2pot');

gulp.task('default', function () {
    return gulp.src('src/*.php')
        .pipe(json2pot( {
            domain: 'domain',
            package: 'Example project'
        } ))
        .pipe(gulp.dest('file.pot'));
});
```


## json2pot({options})

See available options in the json2pot readme, https://github.com/diosney/json2pot#options  
All options except src and writeFile is passed to json2pot.

## Related

- [json2pot](https://github.com/diosney/json2pot) - API for this module

## License

MIT © [Diosney Sarmiento](https://github.com/diosney)

Thanks to [Rasmus Bengtsson](https://github.com/rasmusbe) for its work on 
[wp-pot](https://github.com/rasmusbe/wp-pot) which this package is heavily based on.
