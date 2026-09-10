# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Частен Markdown редактор, който работи офлайн, с живо HTML визуализиране. **Just Render the Markdown, Please** е уеб приложение от един-единствен файл: запазете HTML файла, отворете го в браузър и го използвайте без акаунт, сървър, инсталация или връзка с интернет. Всички данни остават на вашия компютър; нищо не се качва.

[Отваряне на приложението](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Текуща версия: **0.2.0** — показва се в прозореца „Относно“ на приложението.

## Възможности

- Живо визуализиране от Markdown към HTML
- Разделен изглед на компютър: редакторът на Markdown отляво, полученият HTML отдясно
- Изтегляне на готовия документ като пълноценен самостоятелен файл `.html`
- Шест вградени примера на Markdown
- Възможности на Markdown в стила на GitHub, включително таблици, списъци със задачи, зачертан текст, автоматични връзки и заградени блокове с код
- Открояване на синтаксиса за 36 езика в заградените блокове с код — както в редактора, така и в готовия документ
- Суровият HTML е изключен по подразбиране от съображения за сигурност
- Потребителски интерфейс на 40 езика
- Без реклами, регистрация, абонаменти и проследяващи модули

## Теми на документа

Готовият Markdown документ има собствена система от теми, независима от интерфейса на приложението.

Включени теми: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Всяка тема съдържа както светла, така и тъмна палитра.

Падащото меню за режим на документа предлага:

- **Автоматично светло/тъмно** — следва настройката `prefers-color-scheme` на браузъра
- **Винаги тъмно**
- **Винаги светло**

Един и същ генериран CSS се използва както за живото визуализиране, така и за изтегления HTML, така че изнесените документи съответстват на избраната тема и поведение на режима.

## Открояване на синтаксиса

Заградените блокове с код се открояват синтактично, когато оградата посочва език:

    ```python
    print("hello")
    ```

Открояването се осигурява от Highlight.js 11.9.0.

Поддържани езици: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML и YAML.

## Суров HTML

Суровият HTML в Markdown е изключен по подразбиране.

Когато **Разрешаване на суров HTML** е включено, приложението все пак почиства получения резултат преди показване или изнасяне. Почистването премахва или ограничава потенциално опасно съдържание, например:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- формуляри
- атрибути за обработка на събития като `onclick`
- адреси `javascript:`
- друго небезопасно вградено съдържание

Включвайте суров HTML само за Markdown, на който имате доверие.

Освен това визуализацията е изолирана в iframe с включена пясъчна кутия.

## Обработчик на Markdown

Текущата компилация вгражда **Marked 4.0.19** директно в HTML файла, за да работи приложението офлайн.

Кодът на приложението държи обработчика на Markdown зад малък адаптерен слой, което позволява вграденият анализатор да бъде заменен без преработка на останалата част от приложението.

Първоначалната проектна цел беше `markdown-it`; текущата компилация използва браузърния пакет на Marked, наличен по време на изработката.

## Езици

Интерфейсът включва:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Приложението автоматично избира поддържан език според локала на браузъра и поддържа подредба отдясно наляво, където е приложимо.
