---
theme: ./theme
layout: cover
highlighter: shiki
themeConfig:
  primary: '#325AB4'
transition: slide-left
---

# 这是一个标题

部门 - 部门 - 姓名

2023.08.01


---
layout: default
---

#  Introduction

* 这是一个基于 [Slidev](sli.dev) 实现的 Bytedance PPT 模板
* [Slidev](sli.dev) 是一个基于 Markdown 的 PPT 生成工具。优点：
  * 编写 Markdown 即可生成 PPT，<font class="text-primary">关注内容而不是形式</font>
  * 支持来自 icones.js.org 的上万个图标
* 使用本项目必须了解 Markdown：
  * 项目提供了许多模板，大部分情况下，Markdown 就足够了
  * 如果需要个性化页面的样式和元素布局，则需要了解 CSS
  * 如果想自己实现新的模板，则需要了解 Vue
* 下载本项目：https://github.com/imageslr/slidev-bytedance
* 下载原始 PPT 模板：https://bytedance.feishu.cn/file/boxcnTSHNK2b4iFu9GbbCvoluCe

---
layout:center
---

<div class="grid grid-cols-4 h-full text-center">
<SectionNumber :selected="true" index="01" title="标题一" />
<SectionNumber :selected="false" index="02" title="标题二" />
<SectionNumber :selected="false" index="03" title="标题三" />
<SectionNumber :selected="false" index="04" title="标题四" />
</div>

---

# Slide Title

> Slide Subtitle


**bold** foo bar *italic*

**加粗** foo bar *斜体*

* Slide bullet text
  * Slide bullet text
  * Slide bullet text
* Slide bullet text
* Slide bullet text

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Slide Title

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

---
layout: section
---

# Section Title

Section subtitle

---
layout: statement
---

# Statement



---
layout: fact
---

# 100%
Fact Information

---
layout: quote
---

# "Notable quote"
Attribution


---
layout: two-cols
---

# Left
* 1
* 2
* 3


::right::

# Right

This shows on the right

---
layout: image-left
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Code

```ts {all|2|1-6|all}
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = {...user, ...update}  
  saveUser(id, newUser)
}
```

---
src: ./pages/multiple-entries.md
hide: false
---

---
src: ./pages/inspire.md
hide: false
---