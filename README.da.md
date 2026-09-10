# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

En privat Markdown-editor, der virker offline, med live HTML-forhåndsvisning. **Just Render the Markdown, Please** er en webapp i én enkelt fil: gem HTML-filen, åbn den i en browser, og brug den uden konto, server, installation eller internetforbindelse. Alle data bliver på din computer; intet uploades.

[Åbn appen](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Nuværende version: **0.2.0** — vises i appens dialog "Om".

## Funktioner

- Live forhåndsvisning fra Markdown til HTML
- Opdelt visning på computeren: Markdown-editor til venstre, gengivet HTML til højre
- Hent det gengivne dokument som en komplet, selvstændig `.html`-fil
- Seks indbyggede Markdown-eksempler
- Markdown-funktioner i GitHub-stil, blandt andet tabeller, opgavelister, gennemstreget tekst, autolinks og indhegnede kodeblokke
- Syntaksfremhævning for 36 sprog i indhegnede kodeblokke, både i editoren og i det gengivne dokument
- Rå HTML er slået fra som standard af sikkerhedshensyn
- Brugerflade på 40 sprog
- Ingen reklamer, registrering, abonnementer eller sporingsværktøjer

## Dokumenttemaer

Det gengivne Markdown-dokument har sit eget temasystem, uafhængigt af appens brugerflade.

Medfølgende temaer: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Hvert tema indeholder både en lys og en mørk palet.

Rullemenuen for dokumenttilstand tilbyder:

- **Automatisk Lys/Mørk** — følger browserens indstilling `prefers-color-scheme`
- **Altid mørk**
- **Altid lys**

Den samme genererede CSS bruges til både den live forhåndsvisning og den hentede HTML, så eksporterede dokumenter svarer til det valgte tema og tilstandens opførsel.

## Syntaksfremhævning

Indhegnede kodeblokke får syntaksfremhævning, når indhegningen angiver et sprog:

    ```python
    print("hello")
    ```

Fremhævningen drives af Highlight.js 11.9.0.

Understøttede sprog: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML og YAML.

## Rå HTML

Rå HTML i Markdown er slået fra som standard.

Når **Aktivér rå HTML** er slået til, renser appen stadig det gengivne resultat før visning eller eksport. Rensningen fjerner eller begrænser potentielt farligt indhold, såsom:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formularer
- hændelsesattributter som `onclick`
- `javascript:`-adresser
- andet usikkert indlejret indhold

Slå kun rå HTML til for Markdown, du har tillid til.

Den gengivne forhåndsvisning er desuden isoleret i en iframe i sandkassetilstand.

## Markdown-gengiver

Den nuværende udgave indlejrer **Marked 4.0.19** direkte i HTML-filen, så programmet virker offline.

Appens kode holder Markdown-gengiveren bag et lille adapterlag, hvilket gør det muligt at udskifte den indlejrede parser uden at omdesigne resten af appen.

Det oprindelige designmål var `markdown-it`; den nuværende udgave bruger den Marked-browserpakke, der var tilgængelig under udviklingen.

## Sprog

Brugerfladen omfatter:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Appen vælger automatisk et understøttet sprog ud fra browserens sprogindstilling og understøtter højre-mod-venstre-layout, hvor det er relevant.
