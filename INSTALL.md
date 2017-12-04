# w3af 的安装

## 安装前的准备
在开始安装 w3af 之前，需要确认已经安装好以下软件：

- Git 客户端：```sudo apt-get install git```
- Python 2.7（大多数系统默认安装）
- pip 1.1：```sudo apt-get install python-pip```

## 安装
```
git clone https://github.com/andresriancho/w3af.git
cd w3af/
./w3af_console
. /tmp/w3af_dependency_install.sh
```
让我解释一下每一个命令实现了哪些功能：
- 首先使用 ```git``` 下载了 ```w3af``` 的源代码
- 然后尝试运行 ```w3af_console``` 命令，由于缺少依赖项，命令很可能会执行失败。 
执行该命令后将生成一个名为 ```/tmp/w3af_dependency_install.sh``` 的脚本，运行该脚本将安装所必需的依赖项。
- 通过运行 ```/tmp/w3af_dependency_install.sh``` 来安装依赖项

框架的依赖项不会经常改变，如果在更新之后需要新的依赖关系，直接执行该脚本即可。

## 支持的系统
理论上只要能运行Python的系统都可以使用该框架。目前该框架已经在各类Linux发行版、Mac OSX、FreeBSD和OpenBSD进行了测试。


## 相关素材
- [w3af 官方文档：w3af 的安装](http://docs.w3af.org/en/latest/install.html)

