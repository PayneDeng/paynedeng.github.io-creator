---
title: "如何用Hugo搭建博客"
date: 2019-11-30T00:22:26+08:00
draft: false
---

很多语言都可以搭建博客，JS实现的博客生成器叫Hexo（很难用），而Hugo是通过Go语言实现的一个博客生成器，它有个特点，很快，所以今天我用简单的语句就尝试教大家如何在Mac系统下用Hugo搭建一个博客。毕竟前端大师方方说过：

>会抄代码就能搭建博客

# 1.安装Hugo

打开你的iTerm，输入如下代码安装Hugo

```
brew install hugo
hugo version
```

你会得到一个hugo的版本号，我目前的版本是v0.59.1。

# 2.快速搭建博客

## 1.通过官方文档做出网站。

进入[官网](https://gohugo.io/)，点击Quick Start。

## 2.创建一个新站点

```
hugo new site quickstart
```

## 3.添加一个主题

```
cd quickstart
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
echo 'theme = "ananke"' >> config.toml
```

## 4.创建你的第一篇文章

```
hugo new posts/my-first-post.md
```

格式如下：

```
---
title: "My First Post"
date: 2019-03-26T08:47:11+01:00
draft: true
---
```

你可以在`---`后面写下你的第一篇博客的内容。

注意：把`draft`的值从`true`变成`false`意味着你该篇文章的状态从待发布变成了发布。

## 5.启动Hugo服务器

```
hugo server -D
```
出现如下代码

```
                   | EN
+------------------+----+
  Pages            | 10
  Paginator pages  |  0
  Non-page files   |  0
  Static files     |  3
  Processed images |  0
  Aliases          |  1
  Sitemaps         |  1
  Cleaned          |  0

Total in 11 ms
Watching for changes in /Users/bep/quickstart/{content,data,layouts,static,themes}
Watching for config changes in /Users/bep/quickstart/config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

你可以通过`http://localhost:1313/`查看本地预览。

## 6.自定义主题

### 网站配置：

打开`config.toml`编辑：

```
baseURL = "https://example.org/"
languageCode = "en-us"
title = "My New Hugo Site"
theme = "ananke"
```
`languageCode`的值建议改成`zh-Hans`,`title`就是你博客的房间名。

## 7.建立静态页面

```
hugo -D
```
搭建完成，下面可以把它部署到你的网站上去了。

以上。