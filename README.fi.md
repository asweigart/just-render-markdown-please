# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Yksityinen, verkkoyhteydettä toimiva Markdown-editori, jossa on reaaliaikainen HTML-esikatselu. **Just Render the Markdown, Please** on yhden tiedoston verkkosovellus: tallenna HTML-tiedosto, avaa se selaimessa ja käytä sitä ilman tiliä, palvelinta, asennusta tai internetyhteyttä. Kaikki tiedot pysyvät omalla koneellasi; mitään ei lähetetä verkkoon.

[Avaa sovellus](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Nykyinen versio: **0.2.0** — näkyy sovelluksen Tietoja-ikkunassa.

## Ominaisuudet

- Reaaliaikainen esikatselu Markdownista HTML:ksi
- Jaettu näkymä työpöydällä: Markdown-editori vasemmalla, hahmonnettu HTML oikealla
- Hahmonnetun asiakirjan lataaminen täydellisenä, itsenäisenä `.html`-tiedostona
- Kuusi sisäänrakennettua Markdown-esimerkkiä
- GitHub-tyyliset Markdown-ominaisuudet, kuten taulukot, tehtävälistat, yliviivaus, automaattiset linkit ja aidatut koodilohkot
- Syntaksin korostus 36 kielelle aidatuissa koodilohkoissa sekä editorissa että hahmonnetussa asiakirjassa
- Raaka HTML on turvallisuussyistä oletuksena pois käytöstä
- Käyttöliittymä 40 kielellä
- Ei mainoksia, rekisteröitymistä, tilauksia eikä seuraimia

## Asiakirjateemat

Hahmonnetulla Markdown-asiakirjalla on oma teemajärjestelmänsä, joka on riippumaton sovelluksen käyttöliittymästä.

Mukana tulevat teemat: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Jokainen teema sisältää sekä vaalean että tumman väripaletin.

Asiakirjatilan valikko tarjoaa vaihtoehdot:

- **Automaattinen vaalea/tumma** — noudattaa selaimen `prefers-color-scheme`-asetusta
- **Aina tumma**
- **Aina vaalea**

Sama luotu CSS on käytössä sekä reaaliaikaisessa esikatselussa että ladatussa HTML-tiedostossa, joten viedyt asiakirjat vastaavat valittua teemaa ja tilan toimintaa.

## Syntaksin korostus

Aidatut koodilohkot korostetaan, kun aidassa mainitaan kieli:

    ```python
    print("hello")
    ```

Korostuksesta vastaa Highlight.js 11.9.0.

Tuetut kielet: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML ja YAML.

## Raaka HTML

Markdownin sisältämä raaka HTML on oletuksena pois käytöstä.

Kun **Ota raaka HTML käyttöön** on valittuna, sovellus puhdistaa hahmonnetun tuloksen silti ennen näyttämistä tai vientiä. Puhdistin poistaa tai rajoittaa mahdollisesti vaarallista sisältöä, kuten:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- lomakkeet
- tapahtumankäsittelijäattribuutit, kuten `onclick`
- `javascript:`-osoitteet
- muu turvaton upotettu sisältö

Ota raaka HTML käyttöön vain sellaiselle Markdownille, johon luotat.

Hahmonnettu esikatselu on lisäksi eristetty hiekkalaatikkotilassa olevaan iframeen.

## Markdown-hahmonnin

Nykyinen koontiversio upottaa **Marked 4.0.19**:n suoraan HTML-tiedostoon, jotta sovellus toimii ilman verkkoyhteyttä.

Sovelluksen koodi pitää Markdown-hahmontimen pienen sovitinkerroksen takana, joten upotetun jäsentimen voi vaihtaa suunnittelematta sovelluksen muita osia uudelleen.

Alkuperäinen suunnittelutavoite oli `markdown-it`; nykyinen koontiversio käyttää Markedin selainpakettia, joka oli saatavilla toteutushetkellä.

## Kielet

Käyttöliittymän kielet:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Sovellus valitsee tuetun kielen automaattisesti selaimen kieliasetuksen perusteella ja tukee tarvittaessa oikealta vasemmalle etenevää asettelua.
