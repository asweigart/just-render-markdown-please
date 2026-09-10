# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Súkromný offline editor Markdownu so živým náhľadom HTML. **Just Render the Markdown, Please** je webová aplikácia v jedinom súbore: uložte súbor HTML, otvorte ho v prehliadači a používajte bez účtu, servera, inštalácie či pripojenia na internet. Všetky údaje zostávajú vo vašom počítači; nič sa nikam neodosiela.

[Otvoriť aplikáciu](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Aktuálna verzia: **0.2.0** — zobrazuje sa v dialógu „O aplikácii“.

## Funkcie

- Živý náhľad prevodu Markdownu na HTML
- Rozdelené zobrazenie na počítači: editor Markdownu vľavo, vykreslené HTML vpravo
- Stiahnutie vykresleného dokumentu ako úplného samostatného súboru `.html`
- Šesť vstavaných ukážok Markdownu
- Funkcie Markdownu v štýle GitHubu vrátane tabuliek, zoznamov úloh, prečiarknutia, automatických odkazov a ohraničených blokov kódu
- Zvýrazňovanie syntaxe pre 36 jazykov v ohraničených blokoch kódu, a to v editore aj vo vykreslenom dokumente
- Surové HTML je z bezpečnostných dôvodov predvolene vypnuté
- Používateľské rozhranie v 40 jazykoch
- Bez reklám, registrácie, predplatného a sledovacích prvkov

## Motívy dokumentu

Vykreslený dokument Markdownu má vlastný systém motívov, nezávislý od rozhrania aplikácie.

Zahrnuté motívy: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Každý motív obsahuje svetlú aj tmavú paletu.

Rozbaľovacia ponuka režimu dokumentu ponúka:

- **Automaticky svetlý/tmavý** — riadi sa nastavením prehliadača `prefers-color-scheme`
- **Vždy tmavý**
- **Vždy svetlý**

Pre živý náhľad aj pre stiahnuté HTML sa používa rovnaké vygenerované CSS, takže exportované dokumenty zodpovedajú zvolenému motívu a správaniu režimu.

## Zvýrazňovanie syntaxe

Ohraničené bloky kódu sa zvýraznia, keď je pri ohraničení uvedený jazyk:

    ```python
    print("hello")
    ```

O zvýrazňovanie sa stará Highlight.js 11.9.0.

Podporované jazyky: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML a YAML.

## Surové HTML

Surové HTML v Markdowne je predvolene vypnuté.

Keď je zapnutá možnosť **Povoliť surové HTML**, aplikácia napriek tomu vykreslený výsledok pred zobrazením alebo exportom očistí. Filter odstráni alebo obmedzí potenciálne nebezpečný obsah, napríklad:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formuláre
- atribúty obsluhy udalostí, ako je `onclick`
- adresy `javascript:`
- ďalší nebezpečný vložený obsah

Surové HTML zapínajte len pre Markdown, ktorému dôverujete.

Vykreslený náhľad je navyše izolovaný v iframe v režime sandbox.

## Vykresľovač Markdownu

Aktuálne zostavenie vkladá **Marked 4.0.19** priamo do súboru HTML, aby aplikácia fungovala offline.

Kód aplikácie drží vykresľovač Markdownu za malou vrstvou adaptéra, takže vložený analyzátor možno vymeniť bez prepracovania zvyšku aplikácie.

Pôvodným návrhovým cieľom bol `markdown-it`; aktuálne zostavenie používa prehliadačový balík Marked, ktorý bol počas tvorby k dispozícii.

## Jazyky

Rozhranie zahŕňa:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikácia automaticky vyberie podporovaný jazyk podľa miestneho nastavenia prehliadača a tam, kde je to vhodné, podporuje rozloženie sprava doľava.
