# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Bizalmas, offline Markdown-szerkesztő élő HTML-előnézettel. A **Just Render the Markdown, Please** egyetlen fájlból álló webalkalmazás: mentse el a HTML-fájlt, nyissa meg böngészőben, és használja fiók, kiszolgáló, telepítés és internetkapcsolat nélkül. Minden adat a saját számítógépén marad; semmi sem kerül feltöltésre.

[Alkalmazás megnyitása](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Jelenlegi verzió: **0.2.0** — az alkalmazás „Névjegy” ablakában látható.

## Funkciók

- Élő előnézet a Markdownból HTML-be
- Osztott nézet asztali gépen: balra a Markdown-szerkesztő, jobbra a megjelenített HTML
- A megjelenített dokumentum letöltése teljes, önálló `.html` fájlként
- Hat beépített Markdown-példa
- GitHub-stílusú Markdown-funkciók, köztük táblázatok, feladatlisták, áthúzott szöveg, automatikus hivatkozások és kerítéses kódblokkok
- Szintaxiskiemelés 36 nyelvhez a kerítéses kódblokkokban, a szerkesztőben és a megjelenített dokumentumban egyaránt
- A nyers HTML biztonsági okokból alapértelmezetten ki van kapcsolva
- Felhasználói felület 40 nyelven
- Nincsenek hirdetések, regisztráció, előfizetések és nyomkövetők

## Dokumentumtémák

A megjelenített Markdown-dokumentumnak saját, az alkalmazás felületétől független témarendszere van.

Beépített témák: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Minden téma világos és sötét színpalettát is tartalmaz.

A dokumentummód legördülő menüje a következőket kínálja:

- **Automatikus világos/sötét** — a böngésző `prefers-color-scheme` beállítását követi
- **Mindig sötét**
- **Mindig világos**

Az élő előnézet és a letöltött HTML ugyanazt a létrehozott CSS-t használja, így az exportált dokumentumok megfelelnek a kiválasztott témának és módnak.

## Szintaxiskiemelés

A kerítéses kódblokkok szintaxiskiemelést kapnak, ha a kerítés megnevez egy nyelvet:

    ```python
    print("hello")
    ```

A kiemelést a Highlight.js 11.9.0 végzi.

Támogatott nyelvek: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML és YAML.

## Nyers HTML

A Markdownban lévő nyers HTML alapértelmezetten ki van kapcsolva.

Ha a **Nyers HTML engedélyezése** be van kapcsolva, az alkalmazás akkor is megtisztítja a megjelenített eredményt a megjelenítés vagy az exportálás előtt. A tisztító eltávolítja vagy korlátozza a potenciálisan veszélyes tartalmat, például:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- űrlapok
- eseménykezelő attribútumok, például `onclick`
- `javascript:` címek
- egyéb nem biztonságos beágyazott tartalom

A nyers HTML-t csak olyan Markdownhoz kapcsolja be, amelyben megbízik.

A megjelenített előnézet ezenfelül homokozó módú iframe-ben van elkülönítve.

## Markdown-megjelenítő

A jelenlegi változat közvetlenül a HTML-fájlba ágyazza a **Marked 4.0.19**-et, hogy az alkalmazás offline is működjön.

Az alkalmazás kódja egy kis illesztőréteg mögött tartja a Markdown-megjelenítőt, így a beágyazott elemző lecserélhető az alkalmazás többi részének újratervezése nélkül.

Az eredeti tervezési cél a `markdown-it` volt; a jelenlegi változat a készítéskor elérhető Marked böngészőcsomagot használja.

## Nyelvek

A felület nyelvei:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Az alkalmazás a böngésző területi beállítása alapján automatikusan kiválaszt egy támogatott nyelvet, és ahol szükséges, támogatja a jobbról balra irányuló elrendezést.
