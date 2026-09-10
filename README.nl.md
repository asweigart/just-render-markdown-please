# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Een privacyvriendelijke, offline Markdown-editor met een live HTML-voorbeeld. **Just Render the Markdown, Please** is een webapp die uit één bestand bestaat: sla het HTML-bestand op, open het in een browser en gebruik het zonder account, server, installatie of internetverbinding. Alle gegevens blijven op je eigen computer; er wordt niets geüpload.

[App openen](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Huidige versie: **0.2.0** — te zien in het venster "Over" van de app.

## Functies

- Live voorbeeld van Markdown naar HTML
- Gesplitste weergave op de desktop: Markdown-editor links, gerenderde HTML rechts
- Het gerenderde document downloaden als een volledig, op zichzelf staand `.html`-bestand
- Zes ingebouwde Markdown-voorbeelden
- Markdown-functies in GitHub-stijl, waaronder tabellen, takenlijsten, doorhalingen, automatische links en omheinde codeblokken
- Syntaxiskleuring voor 36 talen in omheinde codeblokken, zowel in de editor als in het gerenderde document
- Rauwe HTML staat standaard uit, om veiligheidsredenen
- Gebruikersinterface in 40 talen
- Geen advertenties, registratie, abonnementen of trackers

## Documentthema's

Het gerenderde Markdown-document heeft een eigen themasysteem, los van de interface van de app.

Meegeleverde thema's: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Elk thema bevat zowel een licht als een donker palet.

Het keuzemenu voor de documentmodus biedt:

- **Automatisch Licht/Donker** — volgt de browserinstelling `prefers-color-scheme`
- **Altijd donker**
- **Altijd licht**

Voor het live voorbeeld en de gedownloade HTML wordt dezelfde gegenereerde CSS gebruikt, zodat geëxporteerde documenten overeenkomen met het gekozen thema en modusgedrag.

## Syntaxiskleuring

Omheinde codeblokken krijgen syntaxiskleuring wanneer bij de omheining een taal wordt genoemd:

    ```python
    print("hello")
    ```

De kleuring wordt verzorgd door Highlight.js 11.9.0.

Ondersteunde talen: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML en YAML.

## Rauwe HTML

Rauwe HTML in Markdown staat standaard uit.

Wanneer **Rauwe HTML inschakelen** aanstaat, zuivert de app het gerenderde resultaat nog steeds voordat het wordt getoond of geëxporteerd. De zuivering verwijdert of beperkt mogelijk gevaarlijke inhoud, zoals:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formulieren
- gebeurtenisattributen zoals `onclick`
- `javascript:`-URL's
- andere onveilige ingesloten inhoud

Schakel rauwe HTML alleen in voor Markdown die je vertrouwt.

Het gerenderde voorbeeld wordt bovendien geïsoleerd in een iframe met sandbox.

## Markdown-renderer

De huidige build sluit **Marked 4.0.19** rechtstreeks in het HTML-bestand in, zodat de toepassing offline werkt.

De code van de app houdt de Markdown-renderer achter een kleine adapterlaag, waardoor de ingesloten parser vervangen kan worden zonder de rest van de app opnieuw te ontwerpen.

Het oorspronkelijke ontwerpdoel was `markdown-it`; de huidige build gebruikt de browserbundel van Marked die tijdens het maken beschikbaar was.

## Talen

De interface omvat:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

De app kiest automatisch een ondersteunde taal op basis van de browserlocale en ondersteunt waar van toepassing een rechts-naar-links-indeling.
