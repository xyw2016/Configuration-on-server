
# 怎样去装boost库

boost下载的网址[http://www.boost.org/]

1.解压文件
```
tar zxvf boost_*_*.tar.gz
cd boost_*_*.tar.gz
```
2.运行bootstrap.sh脚本
```
./bootstrap.sh --with-libraries=all --with-toolset=gcc
```
--with-libraries=all: 表示安装所有的库
--with-toolset=gcc： 表示指定编译器编译文件

3.编译boost
```
./b2 toolset=gcc
```
4.安装boost
```
./b2 install --prefix=/home/xyw/boost
```
--prefix: 指定安装的文件夹

5.添加环境变量
```
export BOOST_ROOT="/home/xyw/boost/boost_1_68_0"
export BOOST_LIBRARY_DIRS="/home/xyw/boost/lib"
export BOOST_INCLUDEDIR="/home/xyw/boost/include"
```



