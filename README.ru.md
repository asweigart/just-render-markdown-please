# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Приватный офлайн-редактор Markdown с живым предпросмотром HTML. **Just Render the Markdown, Please** — это веб-приложение из одного файла: сохраните HTML-файл, откройте его в браузере и работайте без учётной записи, сервера, установки и подключения к интернету. Все данные остаются на вашем компьютере, ничего никуда не отправляется.

[Открыть приложение](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Текущая версия: **0.2.0** — показана в диалоге «О программе».

## Возможности

- Живой предпросмотр преобразования Markdown в HTML
- Разделённый вид на компьютере: редактор Markdown слева, готовый HTML справа
- Загрузка готового документа как полноценного автономного файла `.html`
- Шесть встроенных примеров Markdown
- Возможности Markdown в стиле GitHub: таблицы, списки задач, зачёркивание, автоссылки и блоки кода в ограждениях
- Подсветка синтаксиса для 36 языков в блоках кода — и в редакторе, и в готовом документе
- Необработанный HTML по умолчанию отключён из соображений безопасности
- Интерфейс на 40 языках
- Без рекламы, регистрации, подписок и трекеров

## Темы документа

У готового документа Markdown есть собственная система тем, независимая от интерфейса приложения.

Встроенные темы: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Каждая тема содержит светлую и тёмную палитры.

Выпадающий список режима документа предлагает:

- **Авто светлая/тёмная** — следует настройке браузера `prefers-color-scheme`
- **Всегда тёмная**
- **Всегда светлая**

Для живого предпросмотра и для загружаемого HTML используется один и тот же сгенерированный CSS, поэтому экспортированные документы соответствуют выбранной теме и поведению режима.

## Подсветка синтаксиса

Блоки кода подсвечиваются, если в ограждении указан язык:

    ```python
    print("hello")
    ```

Подсветку обеспечивает Highlight.js 11.9.0.

Поддерживаемые языки: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML и YAML.

## Необработанный HTML

Необработанный HTML внутри Markdown по умолчанию отключён.

Когда включён параметр **Включить необработанный HTML**, приложение всё равно очищает результат перед показом или экспортом. Очистка удаляет или ограничивает потенциально опасное содержимое, например:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- формы
- атрибуты-обработчики событий, такие как `onclick`
- URL вида `javascript:`
- прочее небезопасное встроенное содержимое

Включайте необработанный HTML только для Markdown, которому доверяете.

Кроме того, предпросмотр изолирован внутри iframe в режиме песочницы.

## Обработчик Markdown

Текущая сборка встраивает **Marked 4.0.19** прямо в HTML-файл, чтобы приложение работало офлайн.

Код приложения держит обработчик Markdown за небольшим слоем-адаптером, поэтому встроенный парсер можно заменить, не перерабатывая остальное приложение.

Изначально ориентировались на `markdown-it`; текущая сборка использует браузерную сборку Marked, доступную на момент создания.

## Языки

Интерфейс доступен на языках:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Приложение автоматически выбирает поддерживаемый язык по локали браузера и при необходимости поддерживает раскладку справа налево.
