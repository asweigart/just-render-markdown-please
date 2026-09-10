# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Privatan Markdown uređivač koji radi izvan mreže, uz prikaz HTML-a uživo. **Just Render the Markdown, Please** je web-aplikacija u jednoj jedinoj datoteci: spremite HTML datoteku, otvorite je u pregledniku i koristite bez računa, poslužitelja, instalacije ili internetske veze. Svi podaci ostaju na vašem računalu; ništa se ne prenosi na mrežu.

[Otvori aplikaciju](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Trenutna inačica: **0.2.0** — prikazuje se u prozoru „O aplikaciji“.

## Značajke

- Prikaz pretvorbe iz Markdowna u HTML uživo
- Podijeljeni prikaz na računalu: Markdown uređivač lijevo, iscrtani HTML desno
- Preuzimanje iscrtanog dokumenta kao potpune, samostalne `.html` datoteke
- Šest ugrađenih primjera Markdowna
- Značajke Markdowna u stilu GitHuba, uključujući tablice, popise zadataka, precrtani tekst, automatske poveznice i ograđene blokove koda
- Isticanje sintakse za 36 jezika u ograđenim blokovima koda, i u uređivaču i u iscrtanom dokumentu
- Sirovi HTML zadano je isključen radi sigurnosti
- Korisničko sučelje na 40 jezika
- Bez oglasa, registracije, pretplata i alata za praćenje

## Teme dokumenta

Iscrtani Markdown dokument ima vlastiti sustav tema, neovisan o sučelju aplikacije.

Uključene teme: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Svaka tema sadrži i svijetlu i tamnu paletu.

Padajući izbornik načina dokumenta nudi:

- **Automatski svijetlo/tamno** — slijedi postavku preglednika `prefers-color-scheme`
- **Uvijek tamno**
- **Uvijek svijetlo**

Isti generirani CSS koristi se i za prikaz uživo i za preuzeti HTML, pa izvezeni dokumenti odgovaraju odabranoj temi i ponašanju načina rada.

## Isticanje sintakse

Ograđeni blokovi koda dobivaju isticanje sintakse kada ograda navodi jezik:

    ```python
    print("hello")
    ```

Isticanje omogućuje Highlight.js 11.9.0.

Podržani jezici: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML i YAML.

## Sirovi HTML

Sirovi HTML unutar Markdowna zadano je isključen.

Kada je uključena mogućnost **Omogući sirovi HTML**, aplikacija i dalje čisti iscrtani rezultat prije prikaza ili izvoza. Čišćenje uklanja ili ograničava potencijalno opasan sadržaj, poput:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- obrazaca
- atributa za rukovanje događajima poput `onclick`
- adresa `javascript:`
- drugog nesigurnog ugrađenog sadržaja

Sirovi HTML uključite samo za Markdown u koji imate povjerenja.

Iscrtani prikaz dodatno je izoliran unutar iframea u zaštićenom načinu rada.

## Markdown iscrtavač

Trenutna izgradnja ugrađuje **Marked 4.0.19** izravno u HTML datoteku kako bi aplikacija radila izvan mreže.

Kod aplikacije drži Markdown iscrtavač iza malog prilagodnog sloja, što omogućuje zamjenu ugrađenog raščlanjivača bez ponovnog osmišljavanja ostatka aplikacije.

Izvorni cilj dizajna bio je `markdown-it`; trenutna izgradnja koristi preglednički paket Marked dostupan u vrijeme izrade.

## Jezici

Sučelje obuhvaća:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikacija automatski odabire podržani jezik na temelju lokalizacije preglednika i podržava raspored zdesna nalijevo ondje gdje je to primjereno.
