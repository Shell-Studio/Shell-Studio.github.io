---
layout: format
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
key: page-format
---

一下是针对页面维护人员和工作人员的一些写作规范指导和提示，请在上传文章时尽量遵循这些规范并仔细阅读提示，这些提示可能会对你的书写语法很有用:)。

## 语法提示

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
