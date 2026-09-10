# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

En privat Markdown-redigerare som fungerar offline, med direktförhandsgranskning av HTML. **Just Render the Markdown, Please** är en webbapp i en enda fil: spara HTML-filen, öppna den i en webbläsare och använd den utan konto, server, installation eller internetanslutning. All data stannar på din dator; ingenting laddas upp.

[Öppna appen](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Aktuell version: **0.2.0** — visas i appens dialogruta ”Om”.

## Funktioner

- Direktförhandsgranskning från Markdown till HTML
- Delad vy på datorn: Markdown-redigeraren till vänster, renderad HTML till höger
- Ladda ner det renderade dokumentet som en komplett fristående `.html`-fil
- Sex inbyggda Markdown-exempel
- Markdown-funktioner i GitHub-stil, bland annat tabeller, uppgiftslistor, genomstrykning, autolänkar och inhägnade kodblock
- Syntaxmarkering för 36 språk i inhägnade kodblock, både i redigeraren och i det renderade dokumentet
- Rå HTML är avstängd som standard av säkerhetsskäl
- Användargränssnitt på 40 språk
- Inga annonser, ingen registrering, inga prenumerationer och inga spårare

## Dokumentteman

Det renderade Markdown-dokumentet har ett eget temasystem, oberoende av appens gränssnitt.

Medföljande teman: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Varje tema innehåller både en ljus och en mörk palett.

Rullgardinsmenyn för dokumentläge erbjuder:

- **Automatiskt Ljust/Mörkt** — följer webbläsarens inställning `prefers-color-scheme`
- **Alltid mörkt**
- **Alltid ljust**

Samma genererade CSS används för både direktförhandsgranskningen och den nedladdade HTML-filen, så exporterade dokument stämmer med valt tema och lägesbeteende.

## Syntaxmarkering

Inhägnade kodblock syntaxmarkeras när inhägnaden anger ett språk:

    ```python
    print("hello")
    ```

Markeringen drivs av Highlight.js 11.9.0.

Språk som stöds: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML och YAML.

## Rå HTML

Rå HTML i Markdown är avstängd som standard.

När **Aktivera rå HTML** är påslagen sanerar appen ändå det renderade resultatet före visning eller export. Saneringen tar bort eller begränsar potentiellt farligt innehåll, till exempel:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formulär
- händelsehanterarattribut som `onclick`
- `javascript:`-adresser
- annat osäkert inbäddat innehåll

Aktivera bara rå HTML för Markdown du litar på.

Den renderade förhandsgranskningen isoleras dessutom i en iframe i sandlådeläge.

## Markdown-renderare

Den aktuella versionen bäddar in **Marked 4.0.19** direkt i HTML-filen så att appen fungerar offline.

Appens kod håller Markdown-renderaren bakom ett litet adapterlager, vilket gör det möjligt att byta ut den inbäddade tolken utan att göra om resten av appen.

Det ursprungliga designmålet var `markdown-it`; den aktuella versionen använder det webbläsarpaket av Marked som fanns tillgängligt när den byggdes.

## Språk

Gränssnittet omfattar:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Appen väljer automatiskt ett språk som stöds utifrån webbläsarens språkinställning och stöder högerställd layout där det är aktuellt.
