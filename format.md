---
layout: article
aside:
  toc: true
titles:
  # @start locale config
    en      : &EN       Format
    en-GB   : *EN
    en-US   : *EN
    en-CA   : *EN
    en-AU   : *EN
    zh-Hans : &ZH_HANS  规范
    zh      : *ZH_HANS
    zh-CN   : *ZH_HANS
    zh-SG   : *ZH_HANS
    zh-Hant : &ZH_HANT  規範
    zh-TW   : *ZH_HANT
    zh-HK   : *ZH_HANT
    ko      : &KO       규범
    ko-KR   : *KO
    fr      : &FR       Normes
    fr-BE   : *FR
    fr-CA   : *FR
    fr-CH   : *FR
    fr-FR   : *FR
    fr-LU   : *FR
  # @end locale config
modify_date: 2020-07-07
key: page-format
---

以下是针对页面维护人员和工作人员的一些写作规范指导和提示，请在上传文章时尽量遵循这些规范并仔细阅读提示，这些提示可能会对你的书写语法很有用:)。

## 个人活动记录页

该页面将会记录你自己的工作和学习进程，还可以展示你自己技能和成果，并以此互为勉励。

我们建议每一位工作人员都应该有一个个人活动记录页，但并不强求。
{:.warning}

### 规范

注意在 *_posts* 文件夹下按 `年-月-日-名字.md` 的格式创建自己的活动记录页。

请确保有一下内容：

* 个人简介
* 活动记录

并确保YAML中有以下信息：

```
---
title: #你的名字
author: #你的名字
modify_date: 2020-07-07 #修改日期
tags:
 - activity page
---
```

其中`author`元素需要在 *_config.yml* 中配置`author`，请联系网页维护人员是否已经为你配置好，如果没有可以催一下，或者自己配置，配置请参考[这个](https://tianqi.name/jekyll-TeXt-theme/docs/zh/authors)。

注意每次修改时更新 `modify_date` 的值
{:.warning}

维护人员会向你询问一些信息以填入资料，但并非必需的。
{:.info}

### 提示

一些特殊的样式请参考官方的[样例](https://tianqi.name/jekyll-TeXt-theme/samples.html)。

或者参考以下例子：

```
---
layout: article
mode: immersive #在沉浸模式下具有带半透明标题的图像文章标题。
header:
  theme: dark
article_header:
  type: cover
  image:
    src: #文章头图
title: #your name
author: #需和 *_config.yml* 中配置的`author`相同
cover: #文章摘要显示的封面
tags:
 - activity page
---
```

## 语法提示

### 前言

注意使用 `<!--more-->` 来分割前言和正文部分。以下是一个例子：

```md
---
layout: article
title: DD
author: DD
tags:
 - activity page
---

Hello, here is my personal activity record page, I will continue to update my work and learning dynamics here.

<!--more-->

---

## 20-07-05

Today we had a meeting…………
```

### 目录

如果需要显示侧边目录，请在YAML中加入以下属性：

```
---
aside:
  toc: true
---
```

### 封面和头图

如果需要在主页显示一个封面，请在YAML中加入以下属性：

```
---
cover: https://i.loli.net/2020/07/05/S2AglOk7dPpmWxw.jpg #文章摘要显示的封面
---
```

如果需要在文章内显示一个头图，请在YAML中加入以下属性：

```
---
article_header:
  type: cover
  image:
    src: #文章头图
---
```

更多的样式请参考官方的[样例](https://tianqi.name/jekyll-TeXt-theme/samples.html)。

### 附加样式

TeXt 自带有一些特殊效果的样式可以使用：

#### 提示

Success Text.
{:.success}

```md
Success Text.
{:.success}
```

Info Text.
{:.info}

```md
Info Text.
{:.info}
```

Warning Text.
{:.warning}

```md
Warning Text.
{:.warning}
```

Error Text.
{:.error}

```md
Error Text.
{:.error}
```

#### 标签

`success`{:.success}

```md
`success`{:.success}
```

`info`{:.info}

```md
`info`{:.info}
```

`warning`{:.warning}

```md
`warning`{:.warning}
```

`error`{:.error}

```md
`error`{:.error}
```

#### 图片

![TestImage](/assets/images/test.jpg){:.border}

```md
![Image](path-to-image){:.border}
```

![TestImage](/assets/images/test.jpg){:.shadow}

```md
![Image](path-to-image){:.shadow}
```

![TestImage](/assets/images/test.jpg){:.rounded}

```md
![Image](path-to-image){:.rounded}
```

![TestImage](/assets/images/test.jpg){:.circle}

```md
![Image](path-to-image){:.circle}
```

![TestImage](/assets/images/test.jpg){:.circle.shadow}

```md
![Image](path-to-image){:.circle.shadow}
```

#### 音乐

**SoundCloud**

<div>{%- include extensions/soundcloud.html id='586191846' -%}</div>

```html
<div>{%- include extensions/soundcloud.html id='313627932' -%}</div>
```

**id:**
![extensions-soundclound](assets/images/extensions-soundclound.jpg){:height="256px"}

**网易云音乐**

<div>{%- include extensions/netease-cloud-music.html id='29124091' -%}</div>

```html
<div>{%- include extensions/netease-cloud-music.html id='413812448' -%}</div>
```

**id:**
![extensions-netease-cloud-music](assets/images/extensions-netease-cloud-music.jpg){:height="256px"}

#### 视频

**YTB**

<div>{%- include extensions/youtube.html id='WZJ7nSdIbwk' -%}</div>

```html
<div>{%- include extensions/youtube.html id='wbY97-hdD5c' -%}</div>
```

**id:**
![extensions-youtube](assets/images/extensions-youtube.jpg){:height="256px"}

**TED**

<div>{%- include extensions/ted.html id='emily_esfahani_smith_there_s_more_to_life_than_being_happy' -%}</div>

```html
<div>{%- include extensions/ted.html id='emily_esfahani_smith_there_s_more_to_life_than_being_happy' -%}</div>
```

**id:**
![extensions-ted](assets/images/extensions-ted.jpg){:height="256px"}

**BiliBili**

<div>{%- include extensions/bilibili.html id='98297433' -%}</div>

```html
<div>{%- include extensions/bilibili.html id='11091080' -%}</div>
```

**id:**
![extensions-bilibili](assets/images/extensions-bilibili.jpg){:height="256px"}
