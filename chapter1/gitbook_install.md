# 第一节 安装gitbook

## 1 安装npm
[下载地址](https://nodejs.org/en/download/)

- 编译源码：

```shell
cd node-v4.4.2  
./configure
make
sudo make install   #这里一定要加sudo
```

- 查看版本

```shell
$ node -v && npm -v 

```
## 2 安装 gitbook

```shell
sudo npm install -g gitbook-cli && gitbook -V 
```
