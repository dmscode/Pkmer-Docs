---
uid: 20230329145808
title: Obsidian 插件：Easy Tpying
tags: [Obsidian, 插件, 输入, 效率, 自动化]
description: Obsidian 插件：Easy Tpying 自动格式化文本对文档的格式进行规范化，并且美化文档的观感，强优化用户的编辑体验。
author: OS
type: other
draft: false
editable: false
modified: 20230515233930
---

# Obsidian 插件：Easy Tpying

Easy-Typing，是一个 Obsidian 的书写体验增强插件，功能包含编辑时自动格式化文本和符号编辑增强。自动格式化文本对文档的格式进行规范化，并且美化文档的观感，强优化用户的编辑体验。

> [!Note] 插件名片
> - 插件名称：Obsidian Easy Typing
> - 插件作者：Yaozhuwa
> - 插件说明：包含编辑时自动格式化文本和符号编辑增强。自动格式化文本对文档的格式进行规范化，并且美化文档的观感，强优化用户的编辑体验。
> - 插件项目地址：[点我跳转](https://github.com/Yaozhuwa/easy-typing-obsidian)

## 效果&特性

- 首字母大写
- 中英文间插入空格/中文间消除空格/标点与文本间插入空格
- 不同区块间的空格策略
- 自定义正则区块
- 符号配对/删除
    - 符号自动配对
    - 配对符号删除

## 安装

1. 进入 Obsidian 社区插件
2. 搜索 Easy Typing
3. 安装
4. 开启插件

## 功能说明

### 文本自动格式化

基于规则的文本自动格式化：

- 文本自动格式化提供了首字母大写功能。此
- 可以根据用户设置的规则在输入过程中对每一行的特定部分自动添加空格。
	- 在中文和英文之间添加空格；
	- 在文本和英文标点之间添加空格；
	- 在文本和行内公式、行内代码、双向链接之间添加空格；
	- 以及在文本区块和用户自定义正则匹配区块之间添加空格。

![image.png](https://cdn.pkmer.cn/images/638091ac6e79c7f51b304cfead5c34b2_MD5.png!pkmer)

文本自动格式化的总开关如上，关闭后不会再输入过程中自动格式化文本。但是不会影响符号编辑增强的功能，也不会影响插件的内置命令：格式化全文、格式化当前行/当前选中区域。

#### 首字母大写

![image.png](https://cdn.pkmer.cn/images/a0782b68c5569cacb70cf3e90463f4af_MD5.png!pkmer)

- 在英文输入模式下自动将每个句子的首字母大写。
- 用户可以在设置中选择是让首字母大写仅在输入时生效，还是在全局范围内生效。
- 如果选择是让首字母大写仅在输入时生效，用户可以取消自动大写，之后不会再对该字母进行大写。

#### 中英文间插入空格/中文间消除空格/标点与文本间插入空格

文本和标点间自动空格，会智能地在其他文本和英文标点间添加空格。

![image.png](https://cdn.pkmer.cn/images/f1ae0c214f723dbdf78d0087f8c527eb_MD5.png!pkmer)

#### 不同区块间的空格策略

将每个文本行分割成几个区块：文本块、行内公式块、行内代码块、链接块、用户自定义正则匹配块。块与块之间的空格策略可以在设置中改变。

![image.png](https://cdn.pkmer.cn/images/c7f087449a936bfaea6e21e6c1b5f561_MD5.png!pkmer)

| 空格策略             | 说明                                 |
|------------------|------------------------------------|
| 无要求              | 该区块与其他区块间没有空格要求，即空不空格分割都可以         |
| 软空格              | 该区块与其他区块可以由软空格分割，即标点符号也可以作为一种软空格。  |
| 严格空格             | 该区块与其他区块间必须有空格分割。                  |

#### 自定义正则区块

在有些情况下，用户不希望对某特定形式的内容进行格式化，比如 `{}` 内部的内容，或者 `<>` 内部的内容。**本插件可以通过用户自定义正则表达式的方式来让本插件对特定形式的内容不进行格式化**。

### 增强编辑

编辑增强包含了 4 个部分的功能，可以在插件设置中分别设置 4 个功能的打开和关闭：

1. 符号自动配对/删除；
2. 选中文本的符号编辑增强；
3. 连续全角符号转半角符号；
4. Obsidian 语法相关的编辑增强。

#### 基础编辑增强

基础编辑增强功能提供了一些考虑 Obsidian 及 Markdown 语法的编辑增强。

#### 符号配对/删除

符号自动配对即输入成对符号的左半边，插件会自动补全其右半边的内容。比如：输入《|，会得到《|》（竖线|代表光标位置）。

当光标左右为配对符号时，使用退格键删除时，会自动把整个配对符号删除。比如：【|】 按退格键，会变成 |。（竖线|代表光标位置）

## 高级玩法

![image.png](https://cdn.pkmer.cn/images/202305041002627.png!pkmer)

比如默认的规则会把一些格式也自动格式化，就需要添加自定义规则进行排除。

常见的规则有：

- 对链接的内容不格式化，包括本地文件链接、网络连接、obsidian 链接、zotero 链接、ftp 链接
   `(file:///|https?://|ftp://|obsidian://|zotero://|www.)[^\s（）《》。,，！？;；：“”‘’\)\(\[\]\{\}']+|++`
- 对 callout 包裹的内容不格式化
  `\[\!.*?\][-+]{0,1}|-+`
- 对双尖括号包裹的内容不格式化，这样使用类似 templater 语法就不会错误的格式化
  `<.*?>|--`
- 对时间格式不格式化，比如 12:54
  `\d{2}:\d{1,2}|++`
- 对 tag 标签的内容不格式化
  `#[\u4e00-\u9fa5\w\/]+|++`

## 功能延伸

插件跟 Obsidian pangu ，linter 等编辑增强插件有许多功能相似之处，不同的地方在于

- 在 Easy Typing 开启状态下，格式规范是实时进行的。我们需要在输入法中输入拼音字母然后选定中文，在这个过程中如果没有选定词语就删除字母，会在原地留下一个空格。
- Obsidian pangu 和 linter 插件都是在内容输入完成后一键全文规范格式，需要手动操作。
- Easy Typing 的自定义规则功能更强大，适合高级用户使用。