---
title: "HTML入门笔记1"
date: 2019-11-30T12:21:59+08:00
draft: true
---

内容里需要介绍
HTML 是谁发明的
HTML 起手应该写什么
常用的表章节的标签有哪些，分别是什么意思（h1~h6、section、article、main、aside 等等）
全局属性有哪些
常用的内容标签有哪些，分别是什么意思（a、strong、em、code、pre 等等）

1. `HTML`是由 Tim Berners-Lee 发明的。

2. `HTML`起手式是 Emmet 感叹号，你可以在 VS code 中，新建一个`index.html`,再首页输入`!`,再按`tab`键得到如下代码

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

此处建议把`lang`的属性值`en`替换成`zh-CN`

3. 表章节的标签主要包括：

   标题 `h1~h6`  
   章节 `setion`  
   文章 `article`  
   段落 `p`  
   头部 `header`  
   脚部 `footer`  
   主要内容 `main`  
   旁支内容 `aside`  
   划分 `div`

4. 全剧属性主要包括：

   `class`  
   `contenteditable`  
   `hidden`  
   `id`  
   `style`  
   `tabindex`  
   `title`

5. 常用的内容标签主要包括：

   `ol+li` 有序列表  
   `ul+li` 无序列表  
   `dl+dt+dd` 描述列表（图表）  
   `pre` 预定义格式文本（保留格式）  
   `hr` 段落级元素之间的主题转换（分割线）  
   `br` 换行符号  
   `a` 锚元素（可以通向网页、文件、同一页面内的位置、电子邮件地址或任何其他`URL`的超链接）  
   `em` 着重阅读内容（语气重要）  
   `strong` 重要阅读内容（本身重要）  
   `code` 代码（等宽字体显示）  
   `q` 引用元素（quote 缩写，短文本）  
   `blockquote` 块级引用元素（段落级别，可空行）

   以上。
