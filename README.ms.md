# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Penyunting Markdown yang peribadi dan luar talian dengan pratonton HTML secara langsung. **Just Render the Markdown, Please** ialah aplikasi web satu fail: simpan fail HTML, buka dalam pelayar, dan gunakannya tanpa akaun, pelayan, pemasangan atau sambungan internet. Semua data kekal pada komputer anda; tiada apa-apa yang dimuat naik.

[Buka Aplikasi](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Versi semasa: **0.2.0** — dipaparkan dalam dialog "Perihal" aplikasi.

## Ciri-ciri

- Pratonton langsung Markdown kepada HTML
- Paparan terbahagi pada desktop: penyunting Markdown di kiri, HTML terhasil di kanan
- Muat turun dokumen terhasil sebagai fail `.html` yang lengkap dan berdiri sendiri
- Enam contoh Markdown terbina dalam
- Ciri Markdown gaya GitHub, termasuk jadual, senarai tugasan, teks bergaris, pautan automatik dan blok kod berpagar
- Penyerlahan sintaks bagi 36 bahasa dalam blok kod berpagar, dalam penyunting dan dokumen terhasil
- HTML mentah dimatikan secara lalai demi keselamatan
- Antara muka pengguna dalam 40 bahasa
- Tiada iklan, pendaftaran, langganan atau penjejak

## Tema Dokumen

Dokumen Markdown terhasil mempunyai sistem tema tersendiri, berasingan daripada antara muka aplikasi.

Tema disertakan: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Setiap tema mengandungi palet cerah dan gelap.

Menu mod dokumen menyediakan:

- **Cerah/Gelap Automatik** — mengikut tetapan `prefers-color-scheme` pelayar
- **Sentiasa Gelap**
- **Sentiasa Cerah**

CSS terjana yang sama digunakan untuk pratonton langsung dan HTML yang dimuat turun, jadi dokumen yang dieksport sepadan dengan tema dan gelagat mod yang dipilih.

## Penyerlahan Sintaks

Blok kod berpagar diserlahkan sintaksnya apabila pagar menamakan sesuatu bahasa:

    ```python
    print("hello")
    ```

Penyerlahan dikuasakan oleh Highlight.js 11.9.0.

Bahasa yang disokong: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML dan YAML.

## HTML Mentah

HTML mentah dalam Markdown dimatikan secara lalai.

Apabila **Dayakan HTML mentah** dihidupkan, aplikasi tetap membersihkan hasil terhasil sebelum memaparkan atau mengeksportnya. Pembersih membuang atau menyekat kandungan yang berpotensi berbahaya, seperti:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- borang
- atribut pengendali peristiwa seperti `onclick`
- URL `javascript:`
- kandungan terbenam lain yang tidak selamat

Dayakan HTML mentah hanya untuk Markdown yang anda percayai.

Pratonton terhasil turut diasingkan di dalam iframe bermod kotak pasir.

## Pemapar Markdown

Binaan semasa membenamkan **Marked 4.0.19** terus ke dalam fail HTML supaya aplikasi berfungsi di luar talian.

Kod aplikasi meletakkan pemapar Markdown di sebalik satu lapisan penyesuai kecil, membolehkan penghurai terbenam digantikan tanpa mereka bentuk semula bahagian lain aplikasi.

Sasaran reka bentuk asal ialah `markdown-it`; binaan semasa menggunakan berkas pelayar Marked yang tersedia semasa pembinaan.

## Bahasa

Antara muka merangkumi:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikasi memilih bahasa yang disokong secara automatik berdasarkan tetapan wilayah pelayar dan menyokong susun atur kanan ke kiri apabila sesuai.
