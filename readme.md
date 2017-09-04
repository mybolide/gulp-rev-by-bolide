## 安装

```
$ npm install --save-dev gulp-rev-by-bolide
```


## 使用

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
API同gulp-rev  
解决gulp-rev不能自定义输出路径，并去除文件hash后缀
