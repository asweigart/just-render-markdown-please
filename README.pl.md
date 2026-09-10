# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Prywatny, działający offline edytor Markdown z podglądem HTML na żywo. **Just Render the Markdown, Please** to aplikacja internetowa w jednym pliku: zapisz plik HTML, otwórz go w przeglądarce i korzystaj bez konta, serwera, instalacji ani połączenia z internetem. Wszystkie dane pozostają na twoim komputerze; nic nie jest wysyłane.

[Otwórz aplikację](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Bieżąca wersja: **0.2.0** — widoczna w oknie „O programie”.

## Funkcje

- Podgląd konwersji Markdown na HTML na żywo
- Widok podzielony na komputerze: edytor Markdown po lewej, wyrenderowany HTML po prawej
- Pobieranie wyrenderowanego dokumentu jako kompletnego, samodzielnego pliku `.html`
- Sześć wbudowanych przykładów Markdown
- Funkcje Markdown w stylu GitHuba, w tym tabele, listy zadań, przekreślenia, autolinki i bloki kodu w ogrodzeniach
- Podświetlanie składni dla 36 języków w blokach kodu — zarówno w edytorze, jak i w wyrenderowanym dokumencie
- Surowy HTML jest domyślnie wyłączony ze względów bezpieczeństwa
- Interfejs użytkownika w 40 językach
- Bez reklam, rejestracji, subskrypcji i modułów śledzących

## Motywy dokumentu

Wyrenderowany dokument Markdown ma własny system motywów, niezależny od interfejsu aplikacji.

Dostępne motywy: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Każdy motyw zawiera zarówno jasną, jak i ciemną paletę.

Lista trybu dokumentu udostępnia:

- **Auto jasny/ciemny** — podąża za ustawieniem przeglądarki `prefers-color-scheme`
- **Zawsze ciemny**
- **Zawsze jasny**

Podgląd na żywo i pobrany HTML korzystają z tego samego wygenerowanego CSS, więc wyeksportowane dokumenty odpowiadają wybranemu motywowi i zachowaniu trybu.

## Podświetlanie składni

Bloki kodu w ogrodzeniach są podświetlane, gdy ogrodzenie wskazuje język:

    ```python
    print("hello")
    ```

Podświetlanie zapewnia Highlight.js 11.9.0.

Obsługiwane języki: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML i YAML.

## Surowy HTML

Surowy HTML w Markdownie jest domyślnie wyłączony.

Gdy opcja **Włącz surowy HTML** jest włączona, aplikacja i tak oczyszcza wyrenderowany wynik przed wyświetleniem lub wyeksportowaniem. Filtr usuwa lub ogranicza potencjalnie niebezpieczne treści, takie jak:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formularze
- atrybuty obsługi zdarzeń, np. `onclick`
- adresy `javascript:`
- inne niebezpieczne treści osadzone

Włączaj surowy HTML wyłącznie dla Markdowna, któremu ufasz.

Wyrenderowany podgląd jest dodatkowo odizolowany w ramce iframe z piaskownicą.

## Silnik renderujący Markdown

Bieżąca kompilacja osadza **Marked 4.0.19** bezpośrednio w pliku HTML, dzięki czemu aplikacja działa offline.

Kod aplikacji trzyma silnik Markdown za niewielką warstwą adaptera, co pozwala wymienić osadzony parser bez przeprojektowywania reszty aplikacji.

Pierwotnym celem projektowym był `markdown-it`; bieżąca kompilacja korzysta z przeglądarkowego pakietu Marked dostępnego w czasie tworzenia.

## Języki

Interfejs obejmuje:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikacja automatycznie wybiera obsługiwany język na podstawie ustawień regionalnych przeglądarki i obsługuje układ od prawej do lewej tam, gdzie jest to potrzebne.
