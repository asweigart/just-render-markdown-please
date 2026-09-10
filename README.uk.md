# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Приватний офлайн-редактор Markdown із живим попереднім переглядом HTML. **Just Render the Markdown, Please** — це вебзастосунок з одного файлу: збережіть HTML-файл, відкрийте його у браузері й користуйтеся без облікового запису, сервера, встановлення чи підключення до інтернету. Усі дані залишаються на вашому комп'ютері; нічого не завантажується в мережу.

[Відкрити застосунок](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Поточна версія: **0.2.0** — показана у вікні «Про програму».

## Можливості

- Живий попередній перегляд перетворення Markdown на HTML
- Розділений вигляд на комп'ютері: редактор Markdown ліворуч, готовий HTML праворуч
- Завантаження готового документа як повного самодостатнього файлу `.html`
- Шість вбудованих прикладів Markdown
- Можливості Markdown у стилі GitHub: таблиці, списки завдань, закреслення, автопосилання та блоки коду в огорожах
- Підсвічування синтаксису для 36 мов у блоках коду — і в редакторі, і в готовому документі
- Необроблений HTML вимкнено за умовчанням з міркувань безпеки
- Інтерфейс користувача 40 мовами
- Без реклами, реєстрації, підписок і трекерів

## Теми документа

Готовий документ Markdown має власну систему тем, незалежну від інтерфейсу застосунку.

Вбудовані теми: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Кожна тема містить світлу й темну палітри.

Спадне меню режиму документа пропонує:

- **Авто світла/темна** — стежить за налаштуванням браузера `prefers-color-scheme`
- **Завжди темна**
- **Завжди світла**

Для живого перегляду й для завантаженого HTML використовується той самий згенерований CSS, тож експортовані документи відповідають обраній темі та поведінці режиму.

## Підсвічування синтаксису

Блоки коду підсвічуються, якщо в огорожі вказано мову:

    ```python
    print("hello")
    ```

Підсвічування забезпечує Highlight.js 11.9.0.

Підтримувані мови: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML та YAML.

## Необроблений HTML

Необроблений HTML усередині Markdown вимкнено за умовчанням.

Коли ввімкнено параметр **Увімкнути необроблений HTML**, застосунок усе одно очищає готовий результат перед показом або експортом. Очищення вилучає або обмежує потенційно небезпечний вміст, зокрема:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- форми
- атрибути-обробники подій, як-от `onclick`
- URL-адреси `javascript:`
- інший небезпечний вбудований вміст

Вмикайте необроблений HTML лише для Markdown, якому довіряєте.

Крім того, попередній перегляд ізольовано всередині iframe у режимі пісочниці.

## Обробник Markdown

Поточна збірка вбудовує **Marked 4.0.19** просто у HTML-файл, щоб застосунок працював офлайн.

Код застосунку тримає обробник Markdown за невеликим шаром-адаптером, тож вбудований парсер можна замінити, не перепроєктовуючи решту застосунку.

Початковою метою розробки був `markdown-it`; поточна збірка використовує браузерний пакет Marked, доступний під час створення.

## Мови

Інтерфейс доступний такими мовами:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Застосунок автоматично добирає підтримувану мову за локаллю браузера та підтримує розкладку справа наліво там, де це доречно.
