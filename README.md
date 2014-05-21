useSASS
=======

sass依赖ruby，请先安装ruby，1.9.3就可以，可以参看[sass安装](http://www.w3cplus.com/sassguide/install.html)

    gem install sass

##sass编译为css

    sass --watch sass_folder:css_folder


sass_folder -要编译的sass所在文件夹

css_folder  -编译后的css所在文件夹


##CSS编译为sass

    sass-convert --from css --to sass -R .

将CSS转换成Sass，进入到css目录执行上述命令。其中“-R”表示递归，“.”表示当前目录。


##关于Compass

在你组织和管理CSS时，Sass真的很优秀。还有个项目Compass,它在CSS框架中使用混合模式，而不是去修改你的HTML结构或者重新定义你的类名。

    gem install comsass


##练习

可以去下载[bootstrap-sass](https://github.com/twbs/bootstrap-sass),进入/vendor/assets把stylesheets转化为css

    sass --watch stylesheets:css

命令结束就新建了一个css文件夹，里面是编译好的css样式表了。

编译为css样式表后，可以再练习下反编译，进入刚才的css文件夹，执行命令

    sass-convert --from css --to sass -R .

你就会看到反编译的sass文件啦，更具体的实际操作项目中练习吧
