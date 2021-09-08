---
title: "05_content"
authors: ["Bing Hu"]
date: 2021-09-01T00:00:00+08:00
draft: false
---

## <span class="section-num">1</span> 内容组织 {#内容组织}

保持博客文章存放在 content/posts 目录, 例如: content/posts/我的第一篇文章.md
保持简单的静态页面存放在 content 目录, 例如: content/about.md


### <span class="section-num">1.1</span> 本地资源 {#本地资源}

有三种方法来引用图片和音乐等本地资源:
使用页面包中的页面资源. 你可以使用适用于 Resources.GetMatch 的值或者直接使用相对于当前页面目录的文件路径来引用页面资源.
将本地资源放在 assets 目录中, 默认路径是 /assets. 引用资源的文件路径是相对于 assets 目录的.
将本地资源放在 static 目录中, 默认路径是 /static. 引用资源的文件路径是相对于 static 目录的.


## <span class="section-num">2</span> 作者配置 {#作者配置}


### <span class="section-num">2.1</span> 在 mysite/data/authors 下创建个人资料 author<sub>name.toml</sub>，以Alice.toml为例： {#在-mysite-data-authors-下创建个人资料-author-以alice-dot-toml为例}

```toml
link = "https://alice.example.com"
email = "alice@example.com"
name = "Alice"
[zh-cn]
    name = "爱丽丝"
```


### <span class="section-num">2.2</span> 在文章中添加作者 {#在文章中添加作者}

```toml
---
authors: [Alice, Bob, Catherine]
---

```
