# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Un editor de Markdown privat i sense connexió, amb previsualització d'HTML en directe. **Just Render the Markdown, Please** és una aplicació web d'un sol fitxer: deseu el fitxer HTML, obriu-lo en un navegador i feu-lo servir sense compte, servidor, instal·lació ni connexió a internet. Totes les dades es queden al vostre ordinador; no es puja res.

[Obre l'aplicació](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Versió actual: **0.2.0** — es mostra al diàleg «Quant a» de l'aplicació.

## Característiques

- Previsualització en directe de Markdown a HTML
- Vista dividida a l'escriptori: l'editor de Markdown a l'esquerra i l'HTML renderitzat a la dreta
- Baixada del document renderitzat com a fitxer `.html` complet i autònom
- Sis exemples de Markdown integrats
- Funcions de Markdown a l'estil de GitHub, com ara taules, llistes de tasques, text ratllat, enllaços automàtics i blocs de codi delimitats
- Ressaltat de sintaxi per a 36 llenguatges als blocs de codi delimitats, tant a l'editor com al document renderitzat
- L'HTML en brut està desactivat per defecte, per seguretat
- Interfície d'usuari en 40 idiomes
- Sense anuncis, registre, subscripcions ni rastrejadors

## Temes del document

El document Markdown renderitzat té el seu propi sistema de temes, independent de la interfície de l'aplicació.

Temes inclosos: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Cada tema conté una paleta clara i una de fosca.

El menú desplegable de mode del document ofereix:

- **Clar/Fosc automàtic** — segueix la configuració `prefers-color-scheme` del navegador
- **Sempre fosc**
- **Sempre clar**

Es fa servir el mateix CSS generat tant per a la previsualització en directe com per a l'HTML baixat, de manera que els documents exportats coincideixen amb el tema i el comportament de mode seleccionats.

## Ressaltat de sintaxi

Els blocs de codi delimitats es ressalten quan la delimitació indica un llenguatge:

    ```python
    print("hello")
    ```

El ressaltat funciona amb Highlight.js 11.9.0.

Llenguatges compatibles: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML i YAML.

## HTML en brut

L'HTML en brut dins del Markdown està desactivat per defecte.

Quan s'activa **Activa l'HTML en brut**, l'aplicació continua sanejant el resultat renderitzat abans de mostrar-lo o exportar-lo. El sanejador elimina o restringeix continguts potencialment perillosos, com ara:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formularis
- atributs de gestió d'esdeveniments com ara `onclick`
- URL `javascript:`
- altres continguts incrustats insegurs

Activeu l'HTML en brut només per a Markdown de confiança.

A més, la previsualització renderitzada queda aïllada dins d'un iframe en mode entorn de proves.

## Renderitzador de Markdown

La versió actual incrusta **Marked 4.0.19** directament al fitxer HTML perquè l'aplicació funcioni sense connexió.

El codi de l'aplicació manté el renderitzador de Markdown darrere d'una petita capa adaptadora, cosa que permet substituir l'analitzador incrustat sense redissenyar la resta de l'aplicació.

L'objectiu de disseny original era `markdown-it`; la versió actual fa servir el paquet de navegador de Marked disponible durant la construcció.

## Idiomes

La interfície inclou:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

L'aplicació selecciona automàticament un idioma compatible segons la configuració regional del navegador i admet la disposició de dreta a esquerra quan escau.
