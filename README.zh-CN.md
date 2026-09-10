# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

一款注重隐私、可离线使用的 Markdown 编辑器，带有实时 HTML 预览。**Just Render the Markdown, Please** 是一个单文件网页应用：保存该 HTML 文件，在浏览器中打开即可使用，无需账号、服务器、安装或联网。所有数据都保存在你自己的电脑上，不会上传任何内容。

[打开应用](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

当前版本：**0.2.0** —— 可在应用的“关于”对话框中查看。

## 功能

- Markdown 转 HTML 的实时预览
- 桌面端分栏视图：左侧为 Markdown 编辑器，右侧为渲染后的 HTML
- 可将渲染后的文档下载为完整的独立 `.html` 文件
- 内置六个 Markdown 示例
- 支持 GitHub 风格的 Markdown 功能，包括表格、任务列表、删除线、自动链接和围栏代码块
- 围栏代码块支持 36 种语言的语法高亮，编辑器和渲染文档中均有效
- 出于安全考虑，默认禁用原始 HTML
- 40 种语言的用户界面
- 无广告、无注册、无订阅、无追踪器

## 文档主题

渲染后的 Markdown 文档拥有独立于应用界面的主题系统。

内置主题：Clean、GitHub、Book、Minimal、Terminal、Solarized、Monokai、Nord、Sepia、Large Print、Compact、Typewriter

每种主题都包含浅色和深色两套配色。

文档模式下拉菜单提供：

- **自动浅色/深色** —— 跟随浏览器的 `prefers-color-scheme` 设置
- **始终深色**
- **始终浅色**

实时预览与下载的 HTML 使用同一套生成的 CSS，因此导出的文档与所选主题和模式行为一致。

## 语法高亮

当围栏代码块标注了语言时，代码会被语法高亮：

    ```python
    print("hello")
    ```

高亮功能由 Highlight.js 11.9.0 提供。

支持的语言：Bash、C、C++、C#、CSS、Diff、Go、GraphQL、INI/TOML、Java、JavaScript、JSON、Kotlin、Less、Lua、Makefile、Markdown、Objective-C、Perl、PHP、PHP Template、Plain Text、Python、Python REPL、R、Ruby、Rust、SCSS、Shell Session、SQL、Swift、TypeScript、VB.NET、WebAssembly、XML/HTML 和 YAML。

## 原始 HTML

Markdown 中的原始 HTML 默认被禁用。

启用**启用原始 HTML**后，应用在显示或导出前仍会对渲染结果进行净化。净化器会移除或限制可能有危险的内容，例如：

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- 表单
- `onclick` 等事件处理属性
- `javascript:` 链接
- 其他不安全的嵌入内容

请仅对你信任的 Markdown 启用原始 HTML。

渲染预览还被隔离在沙箱化的 iframe 中。

## Markdown 渲染器

当前版本将 **Marked 4.0.19** 直接嵌入 HTML 文件，因此应用可以离线工作。

应用代码将 Markdown 渲染器置于一个小型适配层之后，因此可以在不重新设计应用其余部分的情况下替换所嵌入的解析器。

最初的设计目标是 `markdown-it`；当前版本使用的是构建时可用的 Marked 浏览器打包版本。

## 语言

界面语言包括：

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

应用会根据浏览器区域设置自动选择受支持的语言，并在适用时支持从右到左（RTL）布局。
