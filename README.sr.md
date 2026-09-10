# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Приватни Markdown уређивач који ради ван мреже, са живим HTML приказом. **Just Render the Markdown, Please** је веб апликација од само једне датотеке: сачувајте HTML датотеку, отворите је у прегледачу и користите је без налога, сервера, инсталације или интернет везе. Сви подаци остају на вашем рачунару; ништа се не отпрема.

[Отвори апликацију](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Тренутна верзија: **0.2.0** — приказује се у прозору „О програму“.

## Могућности

- Живи приказ претварања Markdown-а у HTML
- Подељени приказ на рачунару: Markdown уређивач лево, исцртани HTML десно
- Преузимање исцртаног документа као потпуне, самосталне `.html` датотеке
- Шест уграђених Markdown примера
- Markdown могућности у стилу GitHub-а, укључујући табеле, спискове задатака, прецртани текст, аутоматске везе и ограђене блокове кода
- Истицање синтаксе за 36 језика у ограђеним блоковима кода, и у уређивачу и у исцртаном документу
- Сирови HTML је подразумевано искључен из безбедносних разлога
- Кориснички интерфејс на 40 језика
- Без реклама, регистрације, претплата и пратилаца

## Теме документа

Исцртани Markdown документ има сопствени систем тема, независан од интерфејса апликације.

Укључене теме: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Свака тема садржи и светлу и тамну палету.

Падајући списак режима документа нуди:

- **Аутоматски светло/тамно** — прати подешавање прегледача `prefers-color-scheme`
- **Увек тамно**
- **Увек светло**

Исти генерисани CSS користи се и за живи приказ и за преузети HTML, па извезени документи одговарају изабраној теми и понашању режима.

## Истицање синтаксе

Ограђени блокови кода добијају истицање синтаксе када ограда наведе језик:

    ```python
    print("hello")
    ```

Истицање омогућава Highlight.js 11.9.0.

Подржани језици: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML и YAML.

## Сирови HTML

Сирови HTML унутар Markdown-а подразумевано је искључен.

Када је укључена опција **Омогући сирови HTML**, апликација и даље чисти исцртани резултат пре приказа или извоза. Чишћење уклања или ограничава потенцијално опасан садржај, као што су:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- обрасци
- атрибути за руковање догађајима попут `onclick`
- адресе `javascript:`
- други небезбедан уграђени садржај

Сирови HTML укључујте само за Markdown у који имате поверења.

Исцртани приказ додатно је изолован унутар iframe-а у режиму заштићеног окружења.

## Markdown исцртавач

Тренутна изградња уграђује **Marked 4.0.19** директно у HTML датотеку, како би апликација радила ван мреже.

Код апликације држи Markdown исцртавач иза малог слоја прилагођивача, што омогућава замену уграђеног рашчлањивача без поновног обликовања остатка апликације.

Првобитни циљ пројекта био је `markdown-it`; тренутна изградња користи прегледачки пакет Marked који је био доступан током израде.

## Језици

Интерфејс обухвата:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Апликација аутоматски бира подржани језик на основу локалитета прегледача и подржава распоред здесна налево тамо где је то потребно.
