# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Isang pribado at offline na Markdown editor na may live na HTML preview. Ang **Just Render the Markdown, Please** ay isang single-file na web app: i-save ang HTML file, buksan ito sa browser, at gamitin nang walang account, server, pag-install, o koneksyon sa internet. Nananatili sa iyong computer ang lahat ng datos; walang ina-upload.

[Buksan ang App](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Kasalukuyang bersyon: **0.2.0** — makikita sa dialog na "Tungkol dito" ng app.

## Mga Tampok

- Live na preview mula Markdown patungong HTML
- Hating tanawin sa desktop: Markdown editor sa kaliwa, na-render na HTML sa kanan
- I-download ang na-render na dokumento bilang kumpleto at nakatayong `.html` file
- Anim na nakapaloob na halimbawa ng Markdown
- Mga tampok ng Markdown na tulad sa GitHub, kabilang ang mga talahanayan, listahan ng gawain, guhit-sa-gitnang teksto, awtomatikong link, at fenced code block
- Syntax highlighting para sa 36 na wika sa mga fenced code block, sa editor at sa na-render na dokumento
- Naka-off bilang default ang raw HTML para sa kaligtasan
- Interface ng gumagamit sa 40 wika
- Walang ad, pagpaparehistro, subscription, o tracker

## Mga Tema ng Dokumento

May sariling sistema ng tema ang na-render na dokumentong Markdown, hiwalay sa interface ng app.

Kasamang mga tema: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

May maliwanag at madilim na paleta ang bawat tema.

Nag-aalok ang dropdown ng mode ng dokumento ng:

- **Awtomatikong Light/Dark** — sumusunod sa setting na `prefers-color-scheme` ng browser
- **Palaging Dark**
- **Palaging Light**

Iisang binuong CSS ang ginagamit para sa live na preview at sa na-download na HTML, kaya tumutugma ang mga na-export na dokumento sa napiling tema at asal ng mode.

## Syntax Highlighting

Nagkakaroon ng syntax highlighting ang mga fenced code block kapag may nakasaad na wika sa fence:

    ```python
    print("hello")
    ```

Pinapagana ang highlighting ng Highlight.js 11.9.0.

Mga suportadong wika: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML, at YAML.

## Raw HTML

Naka-off bilang default ang raw HTML sa loob ng Markdown.

Kapag naka-on ang **Paganahin ang raw HTML**, nililinis pa rin ng app ang na-render na resulta bago ipakita o i-export. Inaalis o nililimitahan ng panlinis ang mga nilalamang maaaring mapanganib, gaya ng:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- mga form
- mga event-handler attribute gaya ng `onclick`
- mga URL na `javascript:`
- iba pang hindi ligtas na naka-embed na nilalaman

Paganahin lamang ang raw HTML para sa Markdown na pinagkakatiwalaan mo.

Nakahiwalay din ang na-render na preview sa loob ng isang naka-sandbox na iframe.

## Markdown Renderer

Direktang isinasama ng kasalukuyang build ang **Marked 4.0.19** sa HTML file para gumana ang app nang offline.

Pinananatili ng code ng app ang Markdown renderer sa likod ng isang maliit na adapter layer, kaya maaaring palitan ang nakapaloob na parser nang hindi na kailangang muling idisenyo ang iba pang bahagi ng app.

Ang orihinal na target ng disenyo ay `markdown-it`; gumagamit ang kasalukuyang build ng browser bundle ng Marked na magagamit noong ginawa ito.

## Mga Wika

Kabilang sa interface ang:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Awtomatikong pumipili ang app ng suportadong wika batay sa locale ng browser at sumusuporta ito sa RTL na layout kung naaangkop.
