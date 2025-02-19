---
title: "使用 HB 的网站"
linkTitle: "网站"
description: 谁在使用 HB 框架？
date: 2023-09-02T23:39:04+08:00
draft: false
nav_icon:
  vendor: bs
  name: globe
  color: green
series:
  - 文档
categories:
tags:
images:
authors:
  - HB
---

与我们分享你使用 HB 构建的网站，一旦审核通过，你的网站将于我们的主页和本页面进行展示。

## 如何添加我的网站？

于 [/data/sites/](https://github.com/hbstack/site/blob/main/data/sites/) 目录下新建一个数据文件以描述和添加你的站点，然后创建 PR 并等待审查和合并。

{{< bs/alert warning >}}
{{< markdownify >}}
数据文件命名约定：使用域名并将其中的点（`.`）替换为破折号（`-`），比如 `https://example.org/` 应该保存为 `example-org.toml`。
{{< /markdownify >}}
{{< /bs/alert >}}

```toml
url = "https://example.org/"
title = "站点名称"
date = "2023-xx-xx"
# logo = ""
# logo_width = 100
# logo_height = 100
```

| Property | Type | Description |
| -------- | :--: | ----------- |
| `url` | string | 网站 URL，**必填**。 |
| `title` | string | 网站名称，请尽可能短，否则可能会被截断。 |
| `date` | date | 请求添加你的站点时的日期，如 `2023-09-01`，**必填**。 |
| `logo` | string | 网站 logo，可选。|
| `logo_width` | number | Logo 原始宽度，当设置了 `logo` 时则必填。 |
| `logo_height` | number | Logo 原始高度，当设置了 `logo` 时则必填。 |

{{< bs/alert warning >}}
{{< markdownify >}}
URLs **必须**使用 HTTPS 协议，否则我们不会接受你的站点。
{{< /markdownify >}}
{{< /bs/alert >}}

## 正在使用 HB 框架的站点 {.text-center}

{{< sites >}}
