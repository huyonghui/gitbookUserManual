# 第二章 使用gitbook
TO-DO
# 根据目录生成图书结构
TO-DO
## README.md 与 SUMMARY编写
```
README.md 这个文件相当于一本Gitbook的简介。 
touch README.md

SUMMARY.md 这个文件是一本书的目录结构，使用Markdown语法 
touch SUMMARY.md
```
在SUMMARY.md 输入:
```
* [简介](README.md)
* [第一章](chapter1/README.md)
 - [第一节](chapter1/section1.md)
 - [第二节](chapter1/section2.md)
* [第二章](chapter2/README.md)
 - [第一节](chapter2/section1.md)
 - [第二节](chapter2/section2.md)
* [结束](end/README.md)
```
## 生成图书结构

当这个目录文件创建好之后，我们可以使用Gitbook的命令行工具将这个目录结构生成相应的目录及文件：
```
$ gitbook init
```

