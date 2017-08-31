# 第二节 生成静态网页

## 生成静态网站
```shell
$ gitbook build ./ && ls
_book  chapter1  chapter2  end  README.md  SUMMARY.md
or
$ gitbook build ./ [DEST_DIR] #指定输出目录
# 解决无法在章节中跳转的问题
$ gitbook --gitbook v2.6.7 install && gitbook --gitbook v2.6.7 build
```

