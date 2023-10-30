## Electron


Electron是使用JavaScript，HTML和CSS构建跨平台的桌面应用程序框架。 Electron兼容Mac、Windows和Linux，可以构建出三个平台的应用程序。

官网：https://www.electronjs.org/

Github：https://github.com/electron/electron

### 简介

**核心是Chromium、Nodejs Native API**

+ Chromium

基于Chromium实现通过Html、css绘制UI，基于Javascript实现UI组件间交互

+ NodeJs

提供了开发集成、组件管理以及构建环境。

+ Native API



Chromium内核提供了一套UI运行时环境，在Chrome浏览器中，通过URL地址解析远程资源，通过Chromium实现资源文件（html、css、js）的解析与渲染。
可以把基于Electron构建的应用看成一个简单的浏览器，只不过改“浏览器”只是解析本地资源，

NodeJs提供了一套前端开发环境，包括前端模块以及开发依赖。通过nodejs环境，可以实现应用中的模块交互、UI构建、数据通信等。

Electron本身也是NodeJs中的一个模块，通过npm包管理器维护。

### 特色

+ 基于javascript、html、css绘制页面及页面交互
+ 应用跨平台
+ Nodejs生态
+ 整体生态环境及成果物比较丰富

### 缺点

+ 集成了Chromium打包非常大
+ 相比原生环境性能问题
+ 依赖问题，Chromium、Node依赖更新
+ 开发复杂度，技术栈围绕NodeJs与前端各种技术
+ 安全问题
+ 系统资源消耗

### 对比

以前开发桌面端应用的方法：
+ Native 
+ QT  
+ Flutter
+ NW 
+ Electron 
+ Tarui 

### 环境准备

+ 开发工具

+ Electron Fiddle
+ Electron-Forge

+ 开发环境

Nodejs

安装NVM


### 原理

+ Electron 是多进程架构，架构具有以下特点：

  + 由一个主进程和 N 个渲染进程组成
  + 主进程承担主导作用，用于完成各种跨平台和原生交互
  + 渲染进程可以是多个，使用 Web 技术开发，通过浏览器内核渲染页面
  + 主进程和渲染进程通过进程间通信来完成各种功能

+ 进程

 + 主进程
 + 渲染进程
 + 进程间通信(IPC)
 
 
 ### 生态
 
 
 ### 产品
 
 开发人员熟知的Visual Studio Code
 MongoDB桌面版管理工具
 Skype桌面版
 WhatsApp桌面版
 HTTP网络测试工具Postman
 
 
 ### 参考
 
 https://blog.csdn.net/xxxzzzqqq_/article/details/129376917