---
uid: 20230329145808
title: Obsidian 社区插件
tags: []
description: Obsidian 社区插件推荐，优秀插件介绍和使用方法
author: OS
type: other
draft: false
editable: false
modified: 20230522212849
---

# Obsidian 社区插件

Obsidian 允许其他开发者编写第三方插件来扩展 Obsidian 的功能。你可以把这点理解清楚 Chrome 或者 Edge 浏览器一样的扩展。

Obsidian 最强大的地方在于插件系统，即使是官方的一些功能，也是通过插件来实现的。因此插件可以按维护者分为核心插件和社区插件两类。核心插件由官方维护，随着 Obsidian 本体进行发行，社区插件由社区插件开发者维护，通过 Obsidian 插件市场进行发行。插件机制提供了极大的自由度，用户可以随意搭配使用，核心插件可以关闭，社区插件可以不安装，甚至可以延迟加载，按需加载插件。这充分考虑到了不同的人有不同的需求，保证每个人使用 Obsidian 都是定制化，轻量化的。带来自由度的同时，是用户需要自己控制功能的复杂度，并不是插件越多越好，功能越多越好，按需使用在无限制的自由度中才能获得真正的自由。社区相当多的贡献者提供开箱即用库，插件测评，教程文档等分享，适度交流可能会有比较大的收益。

## 用户相关

### 安全模式

默认情况下，Obsidian 将打开安全模式，以保护用户免受潜在的伤害。在安全模式下，Obsidian 不会运行任何第三方插件。

> [!Tip] 提示
> 第三方插件可以访问你电脑上的文件，连接互联网，甚至安装额外的程序。了解更多关于插件安全性的信息，请阅读 [[#插件安全性|此部分]]。

为了安装第三方插件，你需要在 `设置` -> `第三方插件` -> `安全模式` 中关闭安全模式。

### 浏览与安装第三方插件

禁用安全模式后，你可以在 `设置` -> `第三方插件` -> `社区插件` -> `浏览` 中打开第三方插件列表页面，从而找到由社区成员开发的第三方插件。

在这个页面上，插件是按照流行度来排列的，你可以轻松地看到最流行的插件。当然，你也可以通过搜索来寻找特定的插件。找到你感兴趣的插件后，点击插件就可以查看插件的详细信息。在详细信息页面，你可以点击 `安装` 按钮来安装插件。

插件安装后，你可以在 `设置` -> `第三方插件` 下找到已安装的插件。插件需要启用才能生效。当然，你也可以在那里卸载它们。

### 插件安全性

Obsidian 非常重视你的数据安全，这使得我们非常重视安全问题，第三方插件的安全性也包括在内。

由于框架的技术原因，我们无法限制插件的权限或访问级别。同时，由于 Obsidian 是一个免费软件，目前我们仍没有精力人工审查每个插件。

值得庆幸的是，Obsidian 拥有一个氛围良好的社区，因此我们可以依靠社区信任来确保第三方插件的安全性。

一般来说，你可以信任在社区中流行的大多数插件。为了进一步确保插件的安全性，我们要求所有社区插件在 GitHub 上开源。**但是，如果你正在处理重要的数据，我们仍建议你在安装插件前检查插件代码，从而更好地保证数据安全。**你可以在插件的详细信息页面找到插件的 Github 仓库地址。

如果你发现第三方插件有安全漏洞，你可以通过在 GitHub 上添加问题来告知插件作者。如果你认为某个插件是恶意的，请联系我们，让我们调查并删除这个插件。

## 插件列表

无论是初入江湖的软件新手，还是经验丰富的江湖老手，面对一个全新的软件时，都难免会遇到一些问题。

我们深知，软件和插件日新月异，但每个插件又有其独特的特点和使用方法。因此，在使用某个插件前，可能需要了解一些基础原理和概念，以更好地理解其功能和使用方法。这也许需要您进行一些小小的功课，但只要您掌握了这些基础知识，使用该软件就会变得容易和流畅。

除此之外，遇到问题时，我们也为您提供了一些简单又实用的描述，帮助您高效地解决问题。我们相信，无论您是新手还是老手，在经过一些练习和摸索后，都能够掌握使用该软件所需的技能和技巧，并在其中体验到乐趣和便捷。

### 功能增强

- [[calendar]]：添加一个简单的日历视图，用于可视化日记和在不同日记间跳转。
- [[obsidian-tray]]：让 Obsidian 关闭窗口时，可以自动缩小到系统托盘
- [[frontmatter-alias-display]]：让你在文件名下直接看到别名
- [[obsidian-global-search-and-replace]]：给 Obsidian 全库进行文本替换

### 编辑增强

这些插件可直接优化或提升 Obsidian 笔记编辑的用户体验。它们一般会直接应用于笔记编辑窗口，使 Obsidian 的操作界面更加直观、可视化，从而提升用户的使用体验。许多插件中还集成了 callout、可视化操作及浮动目录等功能，让你更容易地浏览、查看和编辑笔记内容。所有这些特性的集成对于 Obsidian 用户来说，可以让用户的操作过程变得更为简单、直观，同时也增加了对用户的使用体验的提升。

- [[editing-toolbar]]：添加一个浮动编辑栏，增强 Obsidian 的可视化编辑体验。
- [[floating-toc]]：在文档左侧生成一个悬浮的目录。
- [[lapel]]：在标题旁边显示标题等级，并提供快捷切换标题等级的能力
- [[cm-editor-syntax-highlight-obsidian]]：允许在 Obsidian 的代码块中针对编程语言显示预设的高亮配色方案
- [[obsidian-comments]]：为笔记增加批注或评论。
- [[creases]]：给 Obsidian 的标题增加折叠和展开的功能。
- [[lapel]]：在标题旁边显示标题等级
- [[highlightr-plugin]]：将小而美的高亮菜单添加到了 Obsidian 中，通过所见即所得的方式，为笔记内容中文本增加高亮颜色。
- [[easy-typing-obsidian]]：包含编辑时自动格式化文本和符号编辑增强。自动格式化文本对文档的格式进行规范化，并且美化文档的观感，强优化用户的编辑体验。
- [[obsidian-latex-suite]]：通过片段、文本扩展和编辑器增强功能，使排版 LaTeX 数学与手写一样快
- [[obsidian-dynamic-highlights]]
- [[multi-column-markdown]]：在 Obsidian 的预览模式下创建包含多列内容的 Markdown 文档
- [[remember-cursor-position]]：记住每个文件光标和滚动位置
- [[cm-typewriter-scroll-obsidian]]：打字机风格的滚动，使视图保持在编辑器的中心
- [[number-headings-obsidian]]：给笔记中的标题自动编号，以及动态目录。
- [[cmenu-plugin]]：提供一个 mini 工具栏，以获得更流畅的写作/编辑体验✍🏽。
- [[code-block-copy]]：在阅读模式中，为代码块右上角添加一个复制按钮，点击后自动复制代码块内容到剪贴板。

### 图像

这些插件致力于大幅强化 Obsidian 笔记中图片的操作体验，并提供诸多实用功能，例如方便地查看和管理笔记中的图片，将网络图片集成到本地，等等。这些插件都极大地丰富了 Obsidian 用户的图片使用体验，使用户可以更加方便地在笔记中插入、编辑和排序图片，并提高他们的使用效率。此外，它们还提供了许多高级功能和实用性的工具，例如图片大小调整、编辑、居中、旋转，以及自动生成文件名等。每一个细节都经过了认真优化，让用户可以获得更为舒适顺畅的图片使用体验。

- [[obsidian-image-toolkit]]：提供笔记中查看图片的基本操作
- [[obsidian-image-caption]]：给图片增加说明题注
- [[obsidian-local-images-plus]]：将你粘贴的网络图片，自定下载到本地并插入到你粘贴的位置
 - [[obsidian-file-link]]：可以很容易地将文件链接添加到笔记中，提供界面化的选择文件

### 目录和大纲类

这些插件和大纲、目录有关，它们提供了：快速生成大纲、目录；快速定位目录；快速修改挪动不同笔记标题下内容的能力。活用这些插件，有助于我们更好的组织和梳理自己笔记的核心脉络。

- [[obsidian-dynamic-toc]]：帮助你在笔记中生成对应的目录
- [[obsidian-plugin-toc]]：帮助你在笔记中生成对应的目录
- [[floating-toc]]：在笔记一侧生成悬浮目录，效果近似你在其他在线文档中看到的一样
- [[obsidian-quiet-outline]]：增强大纲插件，按需自动展开大纲
- [[obsidian-outliner]]
- [[obsidian-zoom]]：通过快捷键，快速聚焦到大纲。并在笔记顶部生成标题的面包屑导航，该面包屑可以交互来定位大纲内容。

### 日期&提醒&任务类

这些 Obsidian 插件为用户提供了丰富的功能和工具，其中包括添加简单日历视图管理、多视图项目管理、提醒待办事项、自然语言插入时间戳、基于进度条的任务管理、看板制作、日程规划、任务归类和可视化最后编辑时间等。这些插件的功能差异明显，可以根据个人或组织需求灵活选择使用，让你的事务管理事半功倍。

- [[calendar]]：为 Obsidian 添加一个简单日历功能
- [[obsidian-projects]]：提供多视图的项目管理，包括 表格、看板、日历、画廊等多种视图样式，以适应不同组织需求
- [[obsidian-reminder-plugin]]：为 Markdown 中的待办事项，添加提醒管理。
- [[nldates-obsidian]]：使用自然语言插入时间戳，并链接对应笔记中
- [[obsidian-tasks-plugin]]
- [[progressbar]]：主要作用是将 progressbar 格式的代码块渲染为基于时间或手动的进度条
- [[obsidian-task-progress-bar]]
- [[obsidian-kanban]]：在 Obsidian 制作看板，可以连接你的笔记
- [[obsidian-day-planner]]：用于从 Markdown 笔记中的任务列表中规划和管理番茄钟计时器
- [[obsidian-task-archiver]]：帮你快速归类待办任务
- [[obsidian-last-modified-timestamp-in-status-bar]]：在状态栏可视化你的最后编辑时间

### 搜索

对于那些每天需要处理大量信息和笔记的用户来说，搜索是一个不可或缺的工具。为了满足用户不同的需求，在 Obsidian 中推出了多个强大的搜索插件，方便用户快速、准确地查找和管理笔记。这些插件操作简单、功能多样，可以根据关键字、标签、时间戳等多种方式进行搜索，快速定位笔记。此外，某些插件还支持高级搜索、全文搜索、模糊搜索等功能，让你更加轻松地处理大量信息和笔记。

- [[fuzzy-chinese-pinyin]]：基于汉语拼音进行模糊搜索
- [[search-on-internet]]：快速在搜索引擎中搜索笔记内容
- [[search-obsidian-in-google]]：让你在谷歌搜索中搜索 Obsidian 中的笔记

### 脚注&引用

- [[better-fn]]：为 Obsidian 注脚增加悬浮展示功能，鼠标指向后，注脚的解释会出现在对应位置

### 链接类

这些 Obsidian 插件可以帮助你强化笔记中链接的使用体验，包括从链接粘贴、自动提取链接标题、显示链接对应的网站图标、增加链接的美化样式，以及将网页 URL 转换为嵌入的预览卡片时样式等等。

- [[supercharged-links-obsidian]]：可帮助您根据笔记元数据（例如标签或 YAML 前言属性）设置保管库中链接的样式。可以自动向链接添加颜色、表情符号或其他样式，使其更醒目的进行导航。
- [[obsidian-auto-link-title]]：自动在粘贴时，提取网页链接标题，创建一个 Markdown 链接形式与正确的标题
- [[url-into-selection]]：使用常规 Ctrl/Cmd+V 将链接（URL）插入到选定的文本中。也可以反过来，通过命令面板/快捷键将文本插入到选定的链接（URL）中
- [[external-favicon]]：可以在不使用任何自定义 CSS 的情况下看到链接对应的网站图标
- [[link-favicon]]：可以在不使用任何自定义 CSS 的情况下看到链接对应的网站图标
- [[obsidian-rich-links]]：为你笔记中的链接，增加美化样式
- [[obsidian-link-embed]]：帮你将网页 URL 转换为嵌入预览卡片样式
- [[auto-card-link]]：自动将链接变成卡片样式

### 阅读和 PDF

- [[obsidian-booknote-plugin]]：让你在 Obsidian 中阅读标注 PDF
- [[obsidian-weread-plugin]]：让 Obsidian 和你的微信阅读联动

### 标签类

- [[tag-wrangler]]：增强的标签管理体验，从标签面板中重命名、合并、切换和搜索标签面面俱到
- [[obsidian-tagfolder]]：通过笔记中的标签，重新组织所有的笔记
- [[obsidian-frontmatter-tag-suggest]]：很好解决记忆标签和快速输入的问题，提供标签自动建议的方法，让你可以键入简单字母来快速联想出来对应的标签

### 表格类

鉴于 Obsidian 以 Markdown 为基础，表格编辑一直以来都是用户反馈的难点。 不过，以下列出的插件，将会帮助你解决这些问题，提高你在表格编辑方面的灵活性和操作性。这些插件以其巧妙的设计和出色的功能加以解决了 Obsidian 表格体验中的许多问题，使得 Obsidian 用户能够更加轻松地编辑和管理表格，并大幅提升你使用 Obsidian 时的效率和愉悦感。

- [[obsidian-sortable]]：提供搜索 Obsidian 设置和插件设置选项的能力
- [[table-editor-obsidian]]：改进了表格导航、格式和操作
- [[obsidian-excel-to-markdown-table]]：可以将来自 Microsoft Excel、Google Sheets、Apple Numbers 和 LibreOffice Calc 的数据粘贴为 Obsidian 编辑器中的 Markdown 表格。

### 脑图

- [[obsidian-mindmap-nextgen]]：用于将笔记预览为 Markmap 思维导图
- [[obsidian-enhancing-mindmap]]：让你在 Osidian 中绘制思维导图、大纲和 PDF 文件标注工具。包括多种模式，包括导图模式，表格模式，类白板模式。

### 绘图

- [[obsidian-excalidraw-plugin]]：在 Obsidian 中 使用 Excalidraw 绘图
- [[mermaid-tools]]：提供一个包含常见 mermaid 语法模板的面板，并且可以自定义

### 视图模式

这些插件跟 Obsidian 提供的多种视图模式有关，让你更加灵活的使用不同的视图模式。

- [[obsidian-view-mode-by-frontmatter]]：自定义每个笔记的视图
- [[obsidian-fullscreen-plugin]]：让笔记编辑器变为聚焦模式，或说全屏化
- [[obsidian-focus-mode]]：为 Obsdian 带来了专注模式

### Frontmatter

- [[frontmatter-alias-display]]：让你的笔记名下直接看到别名
- [[obsidian-metatable]]：美化 frontmatter 的显示样式
- [[obsidian-view-mode-by-frontmatter]]：自定义每个笔记的视图
- [[metaedit]]：帮你快捷管理 Obsidian 的元数据，可以预设 YAML 区域的值
- [[obsidian-meta-bind-plugin]]：让你的笔记具有交互性，通过各种控件修改笔记信息

### 自动化&效率

Obsidian 最具吸引力的特点之一，就是它拥有一个丰富的、逐渐壮大起来的插件生态圈。这些卓越的插件不仅增强了 Obsidian 的功能，而且可以在很大程度上提高你的工作和学习效率，让你从繁琐，重复的码字过程中解脱出来。相信这些插件能够帮助你更高效、便捷地管理和利用笔记，让你的学习、工作和生活更加舒适顺畅。相信下面这些插件能帮到你：

- [[templater-obsidian]]：可以替代核心模板插件的效率神器
- [[QuickAdd]]：组合 Obsidian 里所有操作，低阶使用可可视化自动化操作，高阶使用可编写脚本实现万物互联
- [[obsidian-pangu]]：提供了一个全新的增强型文件管理器
- [[cmdr]]：给 Obsidian 的不同功能区增加自定义快捷按钮
- [[weather-fetcher]]：来获取和插入当前的天气到笔记编辑器的插件
- [[obsidian-auto-template-prompt]]：在创建文件时自动打开一个命令窗口让你插入模板。
- [[file-order]]：允许你快速给文件夹的文件加上数字编号
- [[obs-text-wrapper]]：给选中文本加上 HTML 标签
- [[obsidian-wrap-with-shortcuts]]：给选中文本加上自定义前后缀标签
- [[obsidian-dice-roller]]：在文档任意地方生成需要随机的内容，这些随机的候选项可以你来定义
- [[obsidian-markdown-formatting-assistant-plugin]]：提供笔记编辑器中 快速输入 Markdown 语法的方式，此外还提供了一个命令行界面。该命令行界面平铺展示 OB 常用和所有命令提高工作效率。

### 图标类

- [[obsidian-icons-plugin]]：提供插入图标符号的功能。
- [[obsidian-icon-shortcodes]]：通过键入 emoji 对应的段代码方式，快速筛选和输入。并支持自定义图标集合
- [[obsidian-emoji-toolbar]]：快速搜索表情符号并将其插入到您的编辑器中
- [[obsidian-icon-swapper]]：替换默认内置图标集合准备的，可以批量替换，也可以针对某个单一图标进行替换

### 统计类

- [[novel-word-count]]：在 Obsidian 的文件资源管理器窗格中显示每个文件、文件夹和保险库的字数，以及更多其他信息
- [[better-word-count]]：
- [[file-explorer-note-count]]：增加文件数量统计功能
- [[obsidian-daily-stats]]：自动统计笔记更新修改的热力图

### 美化

对于那些对于审美有着极高追求的你来说，这些插件将会成为你 Obsidian 学习和管理的不可或缺的个性化增强工具。虽然这些插件看似只是小小的工具，但它们却有着强大而独特的功能，能够显著提升 Obsidian UI 和设计中的个性化要素。通过本身定制化的特点和某些极具创意的功能，这些插件将使 Obsidian 更加个性化和符合你的审美标准。

- [[Obsidian-Banners]]：为文档页面添加头图和图标
- [[heading-level-indent]]：能根据标题级别缩进内容，用于创建视觉层次结构，使文档的结构和组织更容易理解
- [[obsidian-hider]]：自定义隐藏界面元素、信息
- [[obsidian-style-settings]]：给主题，插件，css 片段提供样式设置的插件
- [[obsidian-icon-folder]]：允许你添加任何自定义图标 (类型为.svg) 或从图标包中添加到您的文件夹或文件
- [[custom-state-for-task-list]]：优化你的任务样式
- [[optimize-canvas-connections]]：优化 Canvas 中的连接线
- [[obsidian-day-and-night]]：根据设定的时间自动切换浅色和深色主题
- [[obsidian-dynamic-background]]：为 Obsidian 添加动态背景
- [[obsidian-minimal-settings]]：为你 Minimal 主题提供自定义选项
- [[obsidian-file-color]]：让你文件管理多姿多彩

### 文件管理类

善于使用优秀的 Obsidian 插件，能够提高你的笔记管理效率和科学性。下面是一些实用的插件：它们提供了增强型文件管理器、面包屑导航、文件字数展示、窗格历史记录等多种功能，让你可以更高效地组织笔记、轻松浏览笔记目录，实现科学的笔记管理。此外，这些插件还支持多种文件夹展开和统计功能，让你更方便地管理笔记。优秀的笔记管理插件，将为你带来更加便捷、高效的学习和工作体验。

 - [[file-tree-alternative]]：提供了一个全新的增强型文件管理器
 - [[quick-explorer]]：在应用标题栏和笔记标题栏增加面包屑导航功能，提供了笔记和目录快速切换的能力
 - [[novel-word-count]]：在 Obsidian 的文件资源管理器窗格中显示每个文件、文件夹和保险库的字数，以及更多其他信息。
 - [[obsidian-collapse-all-plugin]]：单击对应图标或者使用命令，展开或关闭文件管理器中的文件夹
 - [[pane-relief]]：每个窗格的历史记录、用于窗格移动和导航的快捷键等
 - [[recent-files-obsidian]]：显示最近打开的文件列表
 - [[obsidian-gallery]]：让你的笔记变成画廊
 - [[obsidian-tagfolder]]：通过笔记中的标签，重新组织所有的笔记

### 标签页管理

为了让你更加高效地管理学习和工作中的海量笔记，这里向你推荐几款优秀的 Obsidian 插件，它们为 Obsidian 带来全新的标签页操作方式，提升笔记分类和定位的便捷性。这些插件不仅简单易用、操作方便，还可以让你在使用 Obsidian 时省去不必要的繁琐步骤。无论你是在寻找更高效的笔记组织方式还是提高工作效率，这些插件都会给你带来不同程度的改进和便利。

- [[obsidian-tabs]]：为 Obsidian 增加标签页功能
- [[cycle-through-panes]]：使用 `ctrl + Tab` 循环浏览你打开的 tab，就像在浏览器中浏览标签页一样
- [[close-similar-tabs]]：自动关闭重复打开的标签页，防止标签栏拥挤和冲突

### 工具

- [[find-unlinked-files]]：遍历整个仓库，搜索没有反向链接的文件。它将创建一个文件，其中包含指向这些未链接文件的链接列表
- [[settings-search]]：提供搜索 Obsidian 设置和插件设置选项的能力
- [[nl-fast-image-cleaner]]：快速删除笔记中图片和引用链接
- [[oz-clear-unused-images]]：清除笔记中不再使用的图像以节省空间
- [[obsidian42-brat]]：让你可以安装未上架的插件，主题

### 语言

许多学习者选择使用笔记应用程序以替代传统的纸笔笔记方式。尤其是 Obsidian 这类高效而强大的工具，不仅提供了优秀的笔记编写和管理功能，还有许多插件可供选择，能够满足用户多样化的需求，下面这些你不容错过：

- [[obsidian-markdown-furigana]]：日文学习如何增加假名
- [[japanese-word-splitter]]：添加支持日语分词
- [[obsidian-language-learner]]：事半功倍，辅助你在 Obsidian 英语学习，提供查词，生词等功能
- [[obsidian-spaced-repetition]]：利用遗忘曲线间隔重复复习笔记中的内容

### 插入预览

 - [[surfing]]
 - [[convert-url-to-iframe]]：将任何 URL 转换为网页预览插入到笔记中
 - [[simple-embeds]]：把 Twitter 和 YouTube 网页链接嵌入当前笔记中预览
 - [[mx-bili-plugin]]
 - [[media-extended]]
 - [[search-obsidian-in-google]]：让你在谷歌搜索中搜索 Obsidian 中的笔记
 - [[obsidian-file-link]]：可以很容易地将文件链接添加到笔记中，提供界面化的选择文件

### 第三方集成

 - [[obsidian-custom-frames]]：让你在 Obsidian 中以 iframe 方式将 web 应用程序变成标签页
- [[obsidian-douban-plugin]]：给 Obsidian 增加和豆瓣信息同步的能力
- [[obsidian-weread-plugin]]：让 Obsidian 和你的微信阅读联动
- [[obsidian-to-anki-plugin]]：使用 AnkiConnect 来接收 Obsidian 的闪卡（Flashcards）数据

### AI 相关

- [[obsidian-textgenerator-plugin]]：使用 OpenAI 的模型进行文本生成
