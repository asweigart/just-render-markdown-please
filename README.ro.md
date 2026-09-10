# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Un editor Markdown privat, offline, cu previzualizare HTML în timp real. **Just Render the Markdown, Please** este o aplicație web dintr-un singur fișier: salvați fișierul HTML, deschideți-l într-un browser și folosiți-l fără cont, server, instalare sau conexiune la internet. Toate datele rămân pe calculatorul dumneavoastră; nimic nu este încărcat online.

[Deschide aplicația](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Versiunea curentă: **0.2.0** — afișată în fereastra „Despre” a aplicației.

## Funcționalități

- Previzualizare în timp real din Markdown în HTML
- Vizualizare împărțită pe desktop: editorul Markdown în stânga, HTML-ul randat în dreapta
- Descărcarea documentului randat ca fișier `.html` complet și de sine stătător
- Șase exemple Markdown incluse
- Funcții Markdown în stil GitHub, inclusiv tabele, liste de sarcini, text tăiat, autolegături și blocuri de cod delimitate
- Evidențierea sintaxei pentru 36 de limbaje în blocurile de cod delimitate, atât în editor, cât și în documentul randat
- HTML-ul brut este dezactivat implicit, din motive de securitate
- Interfață pentru utilizator în 40 de limbi
- Fără reclame, înregistrare, abonamente sau urmăritoare

## Teme pentru document

Documentul Markdown randat are propriul sistem de teme, independent de interfața aplicației.

Teme incluse: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Fiecare temă conține atât o paletă luminoasă, cât și una întunecată.

Meniul pentru modul documentului oferă:

- **Luminos/Întunecat automat** — urmează setarea `prefers-color-scheme` a browserului
- **Întotdeauna întunecat**
- **Întotdeauna luminos**

Același CSS generat este folosit atât pentru previzualizarea în timp real, cât și pentru HTML-ul descărcat, astfel încât documentele exportate corespund temei și modului selectate.

## Evidențierea sintaxei

Blocurile de cod delimitate sunt evidențiate atunci când delimitarea indică un limbaj:

    ```python
    print("hello")
    ```

Evidențierea este asigurată de Highlight.js 11.9.0.

Limbaje acceptate: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML și YAML.

## HTML brut

HTML-ul brut din Markdown este dezactivat implicit.

Când opțiunea **Activează HTML brut** este pornită, aplicația tot igienizează rezultatul randat înainte de afișare sau export. Filtrul elimină sau restricționează conținutul potențial periculos, precum:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formulare
- atribute pentru tratarea evenimentelor, cum ar fi `onclick`
- adrese `javascript:`
- alt conținut încorporat nesigur

Activați HTML-ul brut doar pentru Markdown în care aveți încredere.

Previzualizarea randată este, în plus, izolată într-un iframe în regim sandbox.

## Motorul de randare Markdown

Versiunea curentă încorporează **Marked 4.0.19** direct în fișierul HTML, pentru ca aplicația să funcționeze offline.

Codul aplicației ține motorul de randare Markdown în spatele unui mic strat adaptor, ceea ce permite înlocuirea analizorului încorporat fără a reproiecta restul aplicației.

Obiectivul inițial de proiectare era `markdown-it`; versiunea curentă folosește pachetul de browser Marked, disponibil în momentul construirii.

## Limbi

Interfața include:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplicația selectează automat o limbă acceptată, în funcție de setările regionale ale browserului, și acceptă aranjarea de la dreapta la stânga acolo unde este cazul.
