# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

A private, offline Markdown editor with a live HTML preview. **Just Render the Markdown, Please** is a single-file web app: save the HTML file, open it in a browser, and use it without an account, server, installation, or internet connection. All data stays on your computer; nothing is uploaded.

[View the App](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Current version: **0.2.0** — shown in the app's About dialog.

## Features

- Live Markdown-to-HTML preview
- Desktop split view: Markdown editor on the left, rendered HTML on the right
- Download the rendered document as a complete standalone `.html` file
- Six built-in Markdown examples
- GitHub-style Markdown features including tables, task lists, strikethrough, autolinks, and fenced code blocks
- Syntax highlighting for 36 languages in fenced code blocks, in both the editor and the rendered document
- Raw HTML is disabled by default for security
- 40-language user interface
- No ads, registration, subscriptions, or trackers

## Document Themes

The rendered Markdown document has its own theme system independent of the application UI.

Included themes: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Every theme contains both a light and dark palette.

The document-mode dropdown provides:

- **Auto Light/Dark** — follows the browser's `prefers-color-scheme` setting
- **Always Dark**
- **Always Light**

The same generated CSS is used for both the live preview and downloaded HTML, so exported documents match the selected theme and mode behavior.

## Syntax Highlighting

Fenced code blocks are syntax highlighted when the fence names a language:

    ```python
    print("hello")
    ```

Highlighting is powered by Highlight.js 11.9.0.

Supported languages: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML, and YAML.

## Raw HTML

Raw HTML in Markdown is disabled by default.

When **Enable Raw HTML** is turned on, the app still sanitizes the rendered result before displaying or exporting it. The sanitizer removes or restricts potentially dangerous content such as:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- forms
- event-handler attributes such as `onclick`
- `javascript:` URLs
- other unsafe embedded content

Only enable raw HTML for Markdown you trust.

The rendered preview is also isolated inside a sandboxed iframe.

## Markdown Renderer

The current build embeds **Marked 4.0.19** directly in the HTML file so the application works offline.

The application code keeps the Markdown renderer behind a small adapter layer, making it possible to replace the embedded parser without redesigning the rest of the app.

The original design target was `markdown-it`; the current build uses the embedded Marked browser bundle available during construction.

## Languages

The interface includes:

English, Simplified Chinese, Spanish, Arabic, Indonesian, Portuguese, French, Japanese, Russian, German, Hindi, Bengali, Urdu, Korean, Vietnamese, Turkish, Italian, Dutch, Polish, Thai, Persian, Ukrainian, Czech, Malay, Romanian, Greek, Hebrew, Swedish, Filipino, Tamil, Hungarian, Danish, Finnish, Norwegian Bokmål, Slovak, Bulgarian, Serbian, Croatian, Slovenian, and Catalan.

The app automatically selects a supported language based on the browser locale and supports RTL layout where appropriate.

