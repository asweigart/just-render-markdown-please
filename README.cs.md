# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Soukromý offline editor Markdownu s živým náhledem HTML. **Just Render the Markdown, Please** je webová aplikace v jediném souboru: uložte soubor HTML, otevřete jej v prohlížeči a používejte bez účtu, serveru, instalace i připojení k internetu. Všechna data zůstávají ve vašem počítači; nic se nikam neodesílá.

[Otevřít aplikaci](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Aktuální verze: **0.2.0** — zobrazuje se v dialogu „O aplikaci“.

## Funkce

- Živý náhled převodu Markdownu do HTML
- Rozdělené zobrazení na počítači: editor Markdownu vlevo, vykreslené HTML vpravo
- Stažení vykresleného dokumentu jako úplného samostatného souboru `.html`
- Šest vestavěných ukázek Markdownu
- Funkce Markdownu ve stylu GitHubu, včetně tabulek, seznamů úkolů, přeškrtnutí, automatických odkazů a ohraničených bloků kódu
- Zvýrazňování syntaxe pro 36 jazyků v ohraničených blocích kódu, a to v editoru i ve vykresleném dokumentu
- Surové HTML je z bezpečnostních důvodů ve výchozím stavu vypnuté
- Uživatelské rozhraní ve 40 jazycích
- Bez reklam, registrace, předplatného a sledovacích prvků

## Motivy dokumentu

Vykreslený dokument Markdownu má vlastní systém motivů, nezávislý na rozhraní aplikace.

Zahrnuté motivy: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Každý motiv obsahuje světlou i tmavou paletu.

Rozbalovací nabídka režimu dokumentu nabízí:

- **Automaticky světlý/tmavý** — řídí se nastavením prohlížeče `prefers-color-scheme`
- **Vždy tmavý**
- **Vždy světlý**

Pro živý náhled i pro stažené HTML se používá stejné vygenerované CSS, takže exportované dokumenty odpovídají zvolenému motivu a chování režimu.

## Zvýrazňování syntaxe

Ohraničené bloky kódu se zvýrazní, pokud je u ohraničení uveden jazyk:

    ```python
    print("hello")
    ```

O zvýrazňování se stará Highlight.js 11.9.0.

Podporované jazyky: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML a YAML.

## Surové HTML

Surové HTML v Markdownu je ve výchozím stavu vypnuté.

Když je zapnuta volba **Povolit surové HTML**, aplikace přesto vykreslený výsledek před zobrazením i exportem očistí. Filtr odstraní nebo omezí potenciálně nebezpečný obsah, například:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formuláře
- atributy obsluhy událostí, jako je `onclick`
- adresy `javascript:`
- další nebezpečný vložený obsah

Surové HTML zapínejte jen pro Markdown, kterému důvěřujete.

Vykreslený náhled je navíc izolovaný uvnitř iframu v režimu sandboxu.

## Vykreslovač Markdownu

Aktuální sestavení vkládá **Marked 4.0.19** přímo do souboru HTML, aby aplikace fungovala offline.

Kód aplikace drží vykreslovač Markdownu za malou vrstvou adaptéru, takže vložený analyzátor lze vyměnit bez přepracování zbytku aplikace.

Původním návrhovým cílem byl `markdown-it`; aktuální sestavení používá prohlížečový balíček Marked, který byl při tvorbě k dispozici.

## Jazyky

Rozhraní zahrnuje:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikace automaticky vybere podporovaný jazyk podle národního prostředí prohlížeče a tam, kde je to vhodné, podporuje rozvržení zprava doleva.
