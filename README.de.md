# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Ein privater, offline nutzbarer Markdown-Editor mit HTML-Live-Vorschau. **Just Render the Markdown, Please** ist eine Webanwendung aus einer einzigen Datei: HTML-Datei speichern, im Browser öffnen und ohne Konto, Server, Installation oder Internetverbindung verwenden. Alle Daten bleiben auf Ihrem Rechner; nichts wird hochgeladen.

[App öffnen](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Aktuelle Version: **0.2.0** — wird im Dialog „Über“ der App angezeigt.

## Funktionen

- Live-Vorschau von Markdown zu HTML
- Geteilte Ansicht am Desktop: Markdown-Editor links, gerendertes HTML rechts
- Das gerenderte Dokument als vollständige, eigenständige `.html`-Datei herunterladen
- Sechs eingebaute Markdown-Beispiele
- Markdown-Funktionen im GitHub-Stil, darunter Tabellen, Aufgabenlisten, Durchstreichungen, Autolinks und umzäunte Codeblöcke
- Syntaxhervorhebung für 36 Sprachen in umzäunten Codeblöcken, sowohl im Editor als auch im gerenderten Dokument
- Rohes HTML ist aus Sicherheitsgründen standardmäßig deaktiviert
- Benutzeroberfläche in 40 Sprachen
- Keine Werbung, keine Registrierung, keine Abos, keine Tracker

## Dokument-Designs

Das gerenderte Markdown-Dokument hat ein eigenes Design-System, unabhängig von der Benutzeroberfläche der App.

Enthaltene Designs: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Jedes Design enthält sowohl eine helle als auch eine dunkle Palette.

Das Auswahlmenü für den Dokumentmodus bietet:

- **Automatisch Hell/Dunkel** — folgt der Browsereinstellung `prefers-color-scheme`
- **Immer dunkel**
- **Immer hell**

Für die Live-Vorschau und das heruntergeladene HTML wird dasselbe erzeugte CSS verwendet, sodass exportierte Dokumente dem gewählten Design und Modusverhalten entsprechen.

## Syntaxhervorhebung

Umzäunte Codeblöcke werden hervorgehoben, wenn die Umzäunung eine Sprache nennt:

    ```python
    print("hello")
    ```

Die Hervorhebung stammt von Highlight.js 11.9.0.

Unterstützte Sprachen: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML und YAML.

## Rohes HTML

Rohes HTML in Markdown ist standardmäßig deaktiviert.

Wenn **Rohes HTML aktivieren** eingeschaltet ist, bereinigt die App das gerenderte Ergebnis dennoch vor Anzeige oder Export. Die Bereinigung entfernt oder beschränkt potenziell gefährliche Inhalte wie:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- Formulare
- Event-Handler-Attribute wie `onclick`
- `javascript:`-URLs
- sonstige unsichere eingebettete Inhalte

Aktivieren Sie rohes HTML nur für Markdown, dem Sie vertrauen.

Die gerenderte Vorschau ist zusätzlich in einem Sandbox-iframe isoliert.

## Markdown-Renderer

Der aktuelle Build bettet **Marked 4.0.19** direkt in die HTML-Datei ein, damit die Anwendung offline funktioniert.

Der Anwendungscode hält den Markdown-Renderer hinter einer kleinen Adapterschicht, sodass der eingebettete Parser ausgetauscht werden kann, ohne den Rest der App neu zu gestalten.

Ursprüngliches Entwurfsziel war `markdown-it`; der aktuelle Build verwendet das während der Erstellung verfügbare Marked-Browser-Bundle.

## Sprachen

Die Oberfläche umfasst:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Die App wählt anhand der Browsersprache automatisch eine unterstützte Sprache und unterstützt bei Bedarf ein Rechts-nach-links-Layout.
