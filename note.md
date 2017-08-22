
# 建站总结

### step 1
以houchen8902.github.io为名，创建新工程，并选择主题后，项目中有两个文件README.md和_config.yml。
_config.ml中只有一句话`theme: jekyll-theme-cayman`，指定主题为cayman。
README.md显示一篇文章。
这时访问https://houchen8902.github.io/，会显示出网页，头部的标题显示工程名，头部的summary显示工程的description。页面内容显示的是README.md中的内容。而整个页面的格式使用的是_config.yml中指定的cayman。

### step 2
在工程根目录添加index.html文件，里面添加一个标题和一个段落。
此时再访问https://houchen8902.github.io/，整个页面就显示index.html的内容。第一，不再显示README.md，第二，不再使用cayman样式。