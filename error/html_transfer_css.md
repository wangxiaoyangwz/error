# error: /sytles.css HTTP/1.1 404-

我在base.html中引用css使用的是:

`<link rel="stylesheet" href="{{'static','styles.css'}}" type="text/css"  >`

这也是`python web 开发`这本书里用的方法

但是并不起作用，发现是引用.css文件错误

解决：
`<link rel="stylesheet" href="../../static/styles.css" type="text/css"  >`


