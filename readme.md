## ��װ

```
$ npm install --save-dev gulp-rev-by-bolide
```


## ʹ��

```js
const gulp = require('gulp');
const rev = require('gulp-rev-by-bolide');

gulp.task('default', () =>
	gulp.src('src/*.css')
		.pipe(rev())
		.pipe(rev.manifest({
            resPath: distPath
        }))
		.pipe(gulp.dest('dist'))
);
```
APIͬgulp-rev  
���gulp-rev�����Զ������·������ȥ���ļ�hash��׺
