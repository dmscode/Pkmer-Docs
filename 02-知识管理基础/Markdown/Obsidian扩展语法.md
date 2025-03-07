---
uid: 20230516140955
title: Obsidian 扩展语法
tags: []
description: 
author: OS
type: other
draft: false
editable: false
modified: 20230516141955
---

# Obsidian 扩展语法

## 笔记内容引用

引用笔记内容到文本

```Markdown
![[笔记文件名#标题名]]  引用具体笔记某个标题下的全部内容
![[笔记文件名^文本块]]  应用具体笔记下某个文本块的内容
```

## Callout

> Obaidian 0.14.2 版本后增加了 Callout 功能，这个功能就是之前 Admonition (简称 ad 插件) 插件收编的，目前语法跟 Microsoft Docs 一致。之前用 ad 插件设置的提示框可以一键转换成最新的语法样式。

你可以参考英文原版，了解这个功能：[Use callouts](https://help.obsidian.md/How+to/Use+callouts)，也可以阅读下面的中文简要说明

在笔记中直接书写（无需代码块）如下内容：

```markdown
> [!规定的标记]
```

这里规定的标记在对应的文章中查找，标记和样式是对应的。

如果可以输入标题，则这样：

```markdown
> [!规定的标记] 标题内容
```

如果还可以输入内容：

```markdown
> [!规定的标记] 标题内容
> 笔记内容，你会发现和 markdown 中的引用是相同的语法
>
> 比如分段也是这样空一行
```

### 目前支持的样式列表

#### 官方示例

> [!note]
> Here's a callout block.
> It supports **markdown** and [[Internal link|wikilinks]].

> [!abstract]

> [!todo]

> [!info]

> [!tip]

> [!success]

> [!question]

> [!warning]

> [!failure]

> [!danger]

> [!bug]

> [!example]

> [!quote]

除了 info 类型还支持以下类型

- note
- abstract, summary, tldr
- info, todo
- tip, hint, important
- success, check, done
- question, help, faq
- warning, caution, attention
- failure, fail, missing
- danger, error
- bug
- example
- quote, cite

### 提示框的各种用法

- 可以没有内容直接显示标题

> [!TIP] Callouts can have custom titles, which also supports **markdown**!

- 折叠提示框

> [!FAQ]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden until it is expanded.

#### 自定义提示框

可以通过 css 设置 my-callout-type 的样式

```css
.callout[data-callout="my-callout-type"] {
    --callout-color: 0, 0, 0;
    --callout-icon: icon-id;
    --callout-icon: '<svg>...custom svg...</svg>';
}
```

#### 居右对其

> [!error|right-small] 浮動到右側
>
> 小視窗，靠右

扩充 Callouts 的语法，在 Callout 类型后上 Pipe，再輸入下列设定：

> [!tip]+ 语法
>
> [!Callout 类型|left/right-small/medium/large] </br> >[!blank-container|left/right-small/medium/large]

### 扩展阅读

>[!Tip] 关联推荐
>- 如果你觉得 callout 可以服用到其他地方：[[obsidian-list-callouts]]
>- 如果你希望优化样式：[[Callout 样式]]

## 键盘文本语法

键盘文本也不一定非得是键盘按键，也可以作为**着重文本**突出显示。一般适合你要描述**快捷键**，按键有关的时候，推荐使用，当然使用其他强化语法也是可以的。

#### 键盘文本的格式

- **`<kbd>键盘文本</kbd>`**
- **`<kbd>Ctrl</kbd> + <kbd>X</kbd>`**
- **效果：**
  <kbd>Ctrl</kbd> + <kbd>X</kbd>

#### 加粗键盘文本

- **加粗**键盘文本的格式有**两种**：
- `<kbd>**键盘文本**</kbd>`
- `**<kbd>ctrl + x</kbd>**`
- **效果：**
<kbd>ctrl + x</kbd>

## 如何插入视频和音频

以插入 B 站视频为例

1. 找到 B 站相关视频，然后点击分享
2. 复制嵌入代码
例子：`<iframe src="//player.bilibili.com/player.html...." scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>`

![image.png](https://cdn.pkmer.cn/images/20230516141418.png!pkmer)

1. 修改嵌入代码为：`<iframe src="**http:**//[http://player.bilibili.com/player.html...](https://link.zhihu.com/?target=http%3A//player.bilibili.com/player.html...)." scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>`

在 `src=“` 后增加 `http:`

1. 将修改后的嵌入代码复制到 obsidian，执行预览看效果

## Emoji 符号

用一对 : 包裹，里面是 **Emoji** 符号的 **语义化文本**

- **示例：**
- `:smile``:sweat``:cat``:woman_cartwheeling`
  - **效果：**
😀 😅 😺 👩 🤸‍♀️

### 补充

- 不支持上述方式的 MD 编辑器或笔记软件，直接用 **输入法** 输入也是可以的
- **Windows 系统** 用户 **win + .** 就可以输入 Emoji 了
- **Obsidian** 用户可以安装**第三方插件**来支持 **Emoji** 的输入，推荐：
1. [[obsidian-emoji-toolbar]]
2. [[emoji-shortcodes]]
3. [[obsidian-icon-shortcodes]]

## 注释语法

**Markdown** 的  **注释**  和  **HMTL**  一样，注释的内容在  **渲染界面** **不可见** （部分编辑器可见)

### **注释 的格式：**

- `<!-- 这里是注释的内容 -->`
- 注释可以是单行，也可以是多行
- 如果有在使用  **Obsidian**  的，它的注释格式是不一样的
- **`%%这是Obsidian的注释内容%%`**

```text
<!-- 这里是一行注释 -->

<!--
这里是
一段
假装有
很多行的
注释
-->

%%这是一行Obsidian里的注释%%

%%
这里是
一段
假装有
很多行的
Obsidian里的
注释
%%
```

### 示范 (只有切换至 编辑模式 才能看到喔)

%% 这是一行 Obsidian 里的注释%%

%% 这里是 一段 假装有 很多行的 Obsidian 里的 注释 %%
