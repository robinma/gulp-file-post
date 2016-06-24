# gulp-file-post

> Upload file to remote server via http post.

## Install

```
npm install --save-dev gulp-file-post
```

## Example

```js
var gulp = require('gulp');
var upload = require('gulp-file-post');

gulp.task('upload', function() {
  return gulp.src('./publish.zip')
    .pipe(upload({
      url: 'http://wapstatic.kf0309.3g.qq.com/receiver/receiver2.php',
      destDir: '/data/wapstatic/keithytsai/open_zc'
    })
  );
});

```

### options

name | type | description
--- | --- | --- 
url | string | remote server receiver
destDir | string | field of upload file destination in the formdata
{other names} | {any types} | field of other customized names in the formdata except url and destDir

## License

MIT
