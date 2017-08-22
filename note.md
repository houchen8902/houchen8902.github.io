
# 建站总结

### step 1
以houchen8902.github.io为名，创建新工程，并选择主题后，项目中有两个文件README.md和_config.yml。
_config.ml中只有一句话`theme: jekyll-theme-cayman`，指定主题为cayman。
README.md显示一篇文章。
这时访问https://houchen8902.github.io/，会显示出网页，头部的标题显示工程名，头部的summary显示工程的description。页面内容显示的是README.md中的内容。而整个页面的格式使用的是_config.yml中指定的cayman。

### step 2
在工程根目录添加index.html文件，里面添加一个标题和一个段落。
此时再访问https://houchen8902.github.io/，整个页面就显示index.html的内容。第一，不再显示README.md，第二，不再使用cayman样式。

### step 3
为index.html指定样式。
`<link rel="stylesheet" type="text/css" href="./index.css">`
在根目录创建index.css样式表，并为段落修改样式为蓝色，然后在index.html中引用index.css。
此时再访问页面，显示的段落文字颜色就变成了蓝色。

### step 4
添加子页面跳转
添加子页面child.html，在index.html中添加跳转链接，链接使用相对路径接向子页面，如下。
`<a href="./child.html">静夜思*李白</a>`
重新访问页面，可以看到链接，点击会跳转到child.html页面，跳转后的链接地址为`https://houchen8902.github.io/child.html`。

### step 5
添加子页面绝对路径跳转
在根目录创建pages目录，复制child.html到pages目录。在index.html中添加链接，路径使用绝对地址'/pages/child.html'。
重新访问页面，点击使用绝对路径的链接，可以跳转到子页面，子页面链接地址为`https://houchen8902.github.io/pages/child.html`。

### step 6
添加index.md，修改index.html文件名为hello.html，刷新页面，显示的内容为index.md中的内容。
jkeyll会自动解析index.md中的内容并显示，并应用cayman样式。头部显示与step1相同。
说明显示优先级 index.md > README.md。

### step 7
把hello.html修改为index.html，刷新页面，显示的是index.html中的内容，显示效果与step 5相同。
说明显示优先级 index.html > index.md > hello.html