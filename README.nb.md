# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

En privat Markdown-editor som virker uten nett, med direkte HTML-forhåndsvisning. **Just Render the Markdown, Please** er en nettapp i én enkelt fil: lagre HTML-filen, åpne den i en nettleser, og bruk den uten konto, tjener, installasjon eller internettforbindelse. Alle data blir værende på din egen maskin; ingenting lastes opp.

[Åpne appen](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Gjeldende versjon: **0.2.0** — vises i appens «Om»-dialog.

## Funksjoner

- Direkte forhåndsvisning fra Markdown til HTML
- Delt visning på datamaskin: Markdown-editor til venstre, gjengitt HTML til høyre
- Last ned det gjengitte dokumentet som en komplett, selvstendig `.html`-fil
- Seks innebygde Markdown-eksempler
- Markdown-funksjoner i GitHub-stil, blant annet tabeller, oppgavelister, gjennomstreking, autolenker og inngjerdede kodeblokker
- Syntaksutheving for 36 språk i inngjerdede kodeblokker, både i editoren og i det gjengitte dokumentet
- Rå HTML er slått av som standard av sikkerhetshensyn
- Brukergrensesnitt på 40 språk
- Ingen reklame, registrering, abonnementer eller sporere

## Dokumenttemaer

Det gjengitte Markdown-dokumentet har sitt eget temasystem, uavhengig av appens grensesnitt.

Inkluderte temaer: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Hvert tema inneholder både en lys og en mørk palett.

Nedtrekksmenyen for dokumentmodus tilbyr:

- **Automatisk Lys/Mørk** — følger nettleserinnstillingen `prefers-color-scheme`
- **Alltid mørk**
- **Alltid lys**

Den samme genererte CSS-en brukes både til direktevisningen og til den nedlastede HTML-en, slik at eksporterte dokumenter samsvarer med valgt tema og modusatferd.

## Syntaksutheving

Inngjerdede kodeblokker får syntaksutheving når gjerdet oppgir et språk:

    ```python
    print("hello")
    ```

Uthevingen drives av Highlight.js 11.9.0.

Språk som støttes: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML og YAML.

## Rå HTML

Rå HTML i Markdown er slått av som standard.

Når **Slå på rå HTML** er aktivert, renser appen likevel det gjengitte resultatet før visning eller eksport. Renseren fjerner eller begrenser potensielt farlig innhold, som:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- skjemaer
- hendelsesattributter som `onclick`
- `javascript:`-adresser
- annet utrygt innebygd innhold

Slå bare på rå HTML for Markdown du stoler på.

Den gjengitte forhåndsvisningen er dessuten isolert i en iframe i sandkassemodus.

## Markdown-gjengiver

Den gjeldende utgaven bygger inn **Marked 4.0.19** direkte i HTML-filen slik at programmet virker uten nett.

Appkoden holder Markdown-gjengiveren bak et lite adapterlag, noe som gjør det mulig å bytte ut den innebygde parseren uten å utforme resten av appen på nytt.

Det opprinnelige designmålet var `markdown-it`; den gjeldende utgaven bruker nettleserpakken til Marked som var tilgjengelig under utviklingen.

## Språk

Grensesnittet omfatter:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Appen velger automatisk et støttet språk ut fra nettleserens språkinnstilling og støtter høyre-til-venstre-oppsett der det er aktuelt.
