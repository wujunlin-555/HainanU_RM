# HugoBlox模板食用指南
我们作为完全不懂前端的臭电控，直接套模板是最敏捷开发的方法（笑）
这篇md用来记录网站的结构和遇到的一些问题
## 一篇blog构建格式
---
title: 
date: 2025-04-02
author: ''
#external_link: https://github.com
tags:
  - Hugo
---
## 主页面管理
content/_index.md
author/admin
共同控制主页
每个文件夹下的_index.md文件都是这个文件夹所代表的页面的主页。
## 目录管理
config\menuconfig管理导航栏内容，通过url进行跳转。
如何知道要跳转到对应的页面？
如果要前往的是当前页面的一个部分，通过/#name进行跳转
url: /#name
对应的部分要用id进行声明这是要跳转的部分
id: name
如果要跳转的是其他页面，那么不需要#，直接用对应路径即可，也不需要在md中声明id。
### 这是一个块：
（好像要打开源码模式才能正常阅读，直接用md读会缩成一行）
---
  - block: collection
    id: details
    content:
      title: 🦈战队详情
      filters:
        folders:
          - event
    design:
      view: article-list
      columns: 1
---
这个块指定了event这个folder，我们直接用于存放战队详情
---
projects:
  - example
---
功能：这个字段用于将当前内容（如博客文章、演讲等）与一个或多个项目关联起来。
用法：
如果你有一个项目文件夹（例如content/project/example/），并且它包含一个index.md文件，你可以通过设置projects字段来引用它。
例如，如果你的项目文件夹路径是content/project/example/，你可以在当前内容文件中设置：

projects:
  - example
如果你需要关联多个项目，可以将它们列在projects数组中：
projects:
  - example
  - another-project
如果你不需要关联任何项目，可以将projects字段设置为空数组：
projects: []