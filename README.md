# HugoBlox模板食用指南
## blog构建格式
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

<!--START_SECTION:news-->

- [Easily make an academic CV website to get more cites and grow your audience 🚀](https://hugoblox.com/blog/easily-make-academic-website/)
- [What&#39;s new in v5.2?](https://hugoblox.com/blog/whats-new-in-v5.2/)
- [What&#39;s new in v5.1?](https://hugoblox.com/blog/whats-new-in-v5.1/)
- [Version 5.0 (February 2021)](https://hugoblox.com/blog/version-5.0-february-2021/)
- [Version 5.0 Beta 3 (February 2021)](https://hugoblox.com/blog/version-5.0-beta-3-february-2021/)
<!--END_SECTION:news-->
