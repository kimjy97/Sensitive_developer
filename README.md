## 2022/02/16
> cmd에서 'gulp fileinclude' 에러 발생

C:\newTest>gulp fileinclude

[22:27:06] Using gulpfile C:\newTest\gulpfile.js

[22:27:06] Starting 'fileinclude'...

[22:27:06] The following tasks did not complete: fileinclude

[22:27:06] Did you forget to signal async completion?

> gulpfile.js -> gulp.task() 함수 수정

gulp.task('fileinclude', fucntion() { });

-> gulp.task('fileinclude', done => { done(); });
