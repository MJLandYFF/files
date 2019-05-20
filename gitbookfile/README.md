# gitbook使用

我们项目文档，都会使用到gitbook，这可以规范我们的文档。下面内容主要包含了：

- 环境要求
- 下载安装
- 编辑文档
- 预览文档

## 环境要求

NodeJS(v4.0.0及以上)

## 下载安装

使用NPM命令下载安装

```
npm install gitbook-cli -g
```

## 编辑文档

这里推荐的编辑器是Typora，也可以在vsCode中编辑

1、新建一个项目文件夹

```
mkdir (projectName)
cd (projectName)
```

2、初始化项目

```
gitbook init
```

会出现两个文件：

README.md

SUMMARY.md

3、建立目录

编辑SUMMARY.md:

```
# Summary

* [概览](README.md)
* [1.PlusBPM简介](doc1/README.md)
    * [1.1.可以构建什么应用](doc1/可以构建什么应用.md)
    * [1.2.PlusBPM运行环境](doc1/PlusBPM运行环境.md)
    * [1.3.PlusBPM企业应用商店](doc1/PlusBPM企业应用商店.md)
    * [1.4.应用解决方案包](doc1/应用解决方案包.md)
* [2.快速入门](doc2/README.md)
* [3.参考指南](doc3/README.md)
* [4.用户手册](doc4/README.md)
* [5.FAQ](doc5/README.md)
* [6.文档历史记录](doc6/README.md)
```

通过 gitbook init  来创建对应的文件，再编辑对应的md文件

## 预览文档

保存后，在命令提示符中输入

```
gitbook serve
```

在浏览器里访问 http://localhost:4000 就可以看到生成的文档

想要生成html，放在服务器上运行：

```
gitbook build
```

会在项目目录下生成一个_book文件夹，这个文件夹里就是对应的html文件

