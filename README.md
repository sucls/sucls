
## 基于docsify搭建博客

[docsify官网](https://docsify.js.org/)
[github awesome](https://github.com/docsifyjs/awesome-docsify)

## 初始化项目

+ 准备node环境
+ 下载docsify依赖 npm i docsify-cli -g
+ 初始化项目 docsify init docs
+ 启动项目 docsify serve ./docs
+ 访问博客 http://localhost:3000

## 目录结构
```
└── docs/
    ├── _media
    ├── assets
    ├── category
    ├── md
    ├── _coverpage.md
    ├── _sidebar.md
    ├── _navbar.md
    ├── _about.md
    └── index.html
└── README.md    
```

### 目录结构说明

+ _sidebar.md 
 
  目录配置
```javascript
  window.$docsify = {
    loadSidebar: true
  }
```

+ index.html 
 
  用于配置一些网站的基础信息，包括：网站采集、留言板、地址等。
+ _coverpage.md 
 
  用于配置博客首页的介绍信息和网站Logo等

## 选择主题

1. 配置主题地址

## 配置

### 左侧目录配置

1. 在根目录添加_sidebar.md
2. 配置
```
  window.$docsify = {
    loadSidebar: true
  }
``` 
3. 配置显示层级或忽略
   <!-- {docsify-ignore} -->
   <!-- {docsify-ignore-all} -->
   window.$docsify中配置subMaxLevel属性
4. 目录内容
```
  * [主页](/)
  * [导航](/md/guide.md "The greatest guide in the world")
```


### 顶部导航配置

1. 在根目录添加_navbar.md
2. 在index.html加入标签
```html
  <body>
    <nav>
      <a href="#/">EN</a>
      <a href="#/zh-cn/">简体中文</a>
    </nav>
    <div id="app"></div>
  </body>
```
3. 配置
```javascript
  window.$docsify = {
    loadNavbar: true,
    loadNavbar: 'nav.md',
  }
```
4. 目录级顶部导航
   在目录下创建自己的_navbar.md

5. 嵌套
```md
  * Getting started

    * [Quick start](quickstart.md)
    * [Writing more pages](more-pages.md)
    * [Custom navbar](custom-navbar.md)
    * [Cover page](cover.md)

  * Configuration
    * [Configuration](configuration.md)
    * [Themes](themes.md)
    * [Using plugins](plugins.md)
    * [Markdown configuration](markdown.md)
    * [Language highlight](language-highlight.md)
```


## 写文章

## 其他

1. 

2. 

## 发布到gitee 


## 发布到github

## 问题

1. 两个搜索框问题？
   当同时引入docsify.min.js与search.min.js时，会出现两个搜索框

## 缺陷

1. 文章多维度分类
2. 文章打标签标签