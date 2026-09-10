# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Zasebni urejevalnik Markdowna, ki deluje brez povezave, z živim predogledom HTML. **Just Render the Markdown, Please** je spletna aplikacija v eni sami datoteki: shranite datoteko HTML, odprite jo v brskalniku in jo uporabljajte brez računa, strežnika, namestitve ali internetne povezave. Vsi podatki ostanejo v vašem računalniku; nič se ne naloži v splet.

[Odpri aplikacijo](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Trenutna različica: **0.2.0** — prikazana je v pogovornem oknu »O programu«.

## Zmožnosti

- Živi predogled pretvorbe iz Markdowna v HTML
- Razdeljen pogled na računalniku: urejevalnik Markdowna na levi, izrisani HTML na desni
- Prenos izrisanega dokumenta kot popolne, samostojne datoteke `.html`
- Šest vgrajenih primerov Markdowna
- Zmožnosti Markdowna v slogu GitHuba, med njimi razpredelnice, seznami opravil, prečrtano besedilo, samodejne povezave in ograjeni bloki kode
- Poudarjanje skladnje za 36 jezikov v ograjenih blokih kode, tako v urejevalniku kot v izrisanem dokumentu
- Surovi HTML je zaradi varnosti privzeto izklopljen
- Uporabniški vmesnik v 40 jezikih
- Brez oglasov, registracije, naročnin in sledilnikov

## Teme dokumenta

Izrisani dokument Markdown ima svoj sistem tem, neodvisen od vmesnika aplikacije.

Vključene teme: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Vsaka tema vsebuje svetlo in temno paleto.

Spustni seznam načina dokumenta ponuja:

- **Samodejno svetlo/temno** — sledi nastavitvi brskalnika `prefers-color-scheme`
- **Vedno temno**
- **Vedno svetlo**

Za živi predogled in za preneseni HTML se uporablja isti ustvarjeni CSS, zato se izvoženi dokumenti ujemajo z izbrano temo in vedenjem načina.

## Poudarjanje skladnje

Ograjeni bloki kode dobijo poudarjeno skladnjo, kadar ograja navaja jezik:

    ```python
    print("hello")
    ```

Poudarjanje omogoča Highlight.js 11.9.0.

Podprti jeziki: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML in YAML.

## Surovi HTML

Surovi HTML znotraj Markdowna je privzeto izklopljen.

Ko je možnost **Omogoči surovi HTML** vklopljena, aplikacija izrisani rezultat pred prikazom ali izvozom še vedno očisti. Čiščenje odstrani ali omeji morebitno nevarno vsebino, na primer:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- obrazce
- atribute za obravnavo dogodkov, kot je `onclick`
- naslove `javascript:`
- drugo nevarno vdelano vsebino

Surovi HTML vklopite samo za Markdown, ki mu zaupate.

Izrisani predogled je poleg tega izoliran v okviru iframe v peskovniškem načinu.

## Izrisovalnik Markdowna

Trenutna gradnja vdela **Marked 4.0.19** neposredno v datoteko HTML, da aplikacija deluje brez povezave.

Koda aplikacije ohranja izrisovalnik Markdowna za majhno vmesno plastjo, zato je mogoče vdelani razčlenjevalnik zamenjati brez preoblikovanja preostanka aplikacije.

Prvotni cilj zasnove je bil `markdown-it`; trenutna gradnja uporablja brskalniški paket Marked, ki je bil na voljo med izdelavo.

## Jeziki

Vmesnik obsega:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikacija samodejno izbere podprt jezik glede na jezikovno nastavitev brskalnika in tam, kjer je to primerno, podpira postavitev od desne proti levi.
