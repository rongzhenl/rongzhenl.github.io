---
layout:     post
title:      "图片插入测试"
subtitle:   "测试本地预览与 GitHub Pages 图片展示"
date:       2026-03-11 12:00:00
author:     "rongzhenl"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 测试
---

> 本文用于测试 Jekyll 博客中的图片插入方式。

## 图片插入方式

在 Jekyll 博客中插入图片，推荐使用相对路径，这样可以同时满足：
- 本地预览（localhost:4000）
- GitHub Pages 部署后展示

### 方式一：Markdown 语法

使用相对路径引用图片：

```markdown
![图片描述](/img/in-post/post-eleme-pwa/Architecture.png)
```

![图 0](../images/ed9aff283ad3570fc8c73589b2397e4a48adf0440bf83a8e9a1a708e9e388da9.png)  


![图 1](../images/ed9aff283ad3570fc8c73589b2397e4a48adf0440bf83a8e9a1a708e9e388da9.png)  
![图 2](../images/ed9aff283ad3570fc8c73589b2397e4a48adf0440bf83a8e9a1a708e9e388da9.png)  
![图 3](../images/ed9aff283ad3570fc8c73589b2397e4a48adf0440bf83a8e9a1a708e9e388da9.png)  
![图 4](../images/ed9aff283ad3570fc8c73589b2397e4a48adf0440bf83a8e9a1a708e9e388da9.png)  

效果如下：

![架构图](/img/in-post/post-eleme-pwa/Architecture.png)

### 方式二：HTML img 标签

可以控制图片大小和居中等样式：

```html
<img src="/img/in-post/post-eleme-pwa/Lighthouse-after.png" width="600">
```

效果如下：

<img src="/img/in-post/post-eleme-pwa/Lighthouse-after.png" width="600">

### 方式三：居中显示

```html
<center>
    <img src="/img/in-post/post-nextgen-web-pwa/flipkart-1.jpeg" width="500">
</center>
```

效果如下：

<center>
    <img src="/img/in-post/post-nextgen-web-pwa/flipkart-1.jpeg" width="500">
</center>

## 多图展示

| 图片 | 说明 |
|:---:|:---|
| ![Lighthouse优化前](/img/in-post/post-eleme-pwa/Lighthouse-before.png) | 优化前 |
| ![Lighthouse优化后](/img/in-post/post-eleme-pwa/Lighthouse-after.png) | 优化后 |

## 图片路径说明

项目中图片统一存放在 `/img/in-post/` 目录下：

```
img/
└── in-post/
    ├── post-eleme-pwa/          # Eleme PWA 相关图片
    ├── post-nextgen-web-pwa/    # PWA 相关图片
    ├── post-wmu/                # 其他图片
    └── ...
```

**关键点：**
1. 路径以 `/img/` 开头（绝对路径，相对于网站根目录）
2. 不要使用 `../img/` 这种相对路径
3. 这样无论是本地 `localhost:4000` 还是 GitHub Pages `rongzhenl.github.io` 都能正确展示

---

测试完成！
