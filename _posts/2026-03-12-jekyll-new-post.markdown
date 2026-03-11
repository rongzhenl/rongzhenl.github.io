---
layout:     post
title:      "Jekyll 新文章测试"
subtitle:   "使用正确的命名规范创建文章"
date:       2026-03-12 10:00:00 +0800
author:     "rongzhenl"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - Jekyll
    - 测试
---

> 本文用于测试 Jekyll 新文章是否正常显示。

## Jekyll 文章命名规范

Jekyll 要求 `_posts` 目录下的文章文件名必须遵循以下格式：

```
YEAR-MONTH-DAY-title.MARKUP
```

例如：`2026-03-12-jekyll-new-post.markdown`

### 注意事项

1. **日期格式**：必须是 `YYYY-MM-DD`
2. **标题**：使用小写字母和连字符，避免空格和特殊字符
3. **扩展名**：`.markdown` 或 `.md`

## 服务启动

`bundle exec jekyll serve -w -l --host 0.0.0.0`


