# 第三节 制作pdf

# 输出PDF
>  phantomjs: <br> 官网参见[http://phantomjs.org/download.html](http://phantomjs.org/download.html)<br>镜像参见[http://npm.taobao.org/dist/phantomjs/](http://npm.taobao.org/dist/phantomjs/)

```shell
# 解压phantomjs压缩包
$ sudo cp bin/phantomjs /bin/ #手动安装phantomjs工具
$ sudo apt-get install calibre #安装生成PDF的依赖库
$ gitbook pdf . && ls
book.pdf  chapter1  chapter2  end  README.md  SUMMARY.md
```

