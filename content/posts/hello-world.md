---
author: "BeiYu"
title: "Hello World"
date: "2022-01-16"
description: "Guide to Hugo-PaperMod-Template"
tags: ["emoji"]
ShowToc: false
math: true
ShowBreadCrumbs: false
---

# Markdown
## 标题

共有6级标题

# H1

## H2

### H3

#### H4

##### H5

###### H6

## 段落

这是第一段，bulabulabula

这是第二段，bulabulabula

## 引用

这是行内引用`inline`

> 这是一个段引用和脚标的栗子
>
> — <cite>出处[^1]</cite>

[^1]: 这是一个脚标的栗子

## 表格

| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |


## 代码块

```python
import os
print("hello world")
```

## 列表

#### 有序列表

1. First item
2. Second item
3. Third item

#### 无序列表

-   List item
-   Another item
-   And another item

## KaTeX

{{< math.inline >}}
{{ if or .Page.Params.math .Site.Params.math }}

<!-- KaTeX -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css" integrity="sha384-zB1R0rpPzHqg7Kpt0Aljp8JPLqbXI3bhnPWROx27a9N0Ll6ZP/+DiW/UqRcLbRjq" crossorigin="anonymous">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.js" integrity="sha384-y23I5Q6l+B6vatafAwxRu/0oK/79VlbSz7Q9aiSZUvyWYIYsd+qj+o24G5ZU2zJz" crossorigin="anonymous"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/contrib/auto-render.min.js" integrity="sha384-kWPLUVMOks5AQFrykwIup5lo0m3iMkkHrD0uJ4H5cjeGihAutqP0yW0J6dpFiVkI" crossorigin="anonymous" onload="renderMathInElement(document.body);"></script>
{{ end }}
{{</ math.inline >}}

{{< math.inline >}}

<p>
Inline math: \(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\)
</p>
{{</ math.inline >}}

Block math:

$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
$$


## Emoji

可以直接输入Emoji表情，或者使用[shortcode](http://www.emoji-cheat-sheet.com/)

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>


## 夜间模式

## RSS

[link](https://lopins.github.io/hugo-template/index.xml)