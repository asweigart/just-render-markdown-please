# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Editor Markdown yang privat dan luring dengan pratinjau HTML langsung. **Just Render the Markdown, Please** adalah aplikasi web satu berkas: simpan berkas HTML-nya, buka di peramban, dan gunakan tanpa akun, server, pemasangan, atau koneksi internet. Semua data tetap di komputer Anda; tidak ada yang diunggah.

[Buka Aplikasi](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Versi saat ini: **0.2.0** — ditampilkan pada dialog "Tentang" di aplikasi.

## Fitur

- Pratinjau langsung Markdown ke HTML
- Tampilan terbagi di desktop: editor Markdown di kiri, HTML hasil render di kanan
- Unduh dokumen hasil render sebagai berkas `.html` mandiri yang lengkap
- Enam contoh Markdown bawaan
- Fitur Markdown bergaya GitHub, termasuk tabel, daftar tugas, teks tercoret, tautan otomatis, dan blok kode berpagar
- Penyorotan sintaksis untuk 36 bahasa pada blok kode berpagar, baik di editor maupun di dokumen hasil render
- HTML mentah dinonaktifkan secara bawaan demi keamanan
- Antarmuka pengguna dalam 40 bahasa
- Tanpa iklan, pendaftaran, langganan, atau pelacak

## Tema Dokumen

Dokumen Markdown hasil render memiliki sistem tema tersendiri, terpisah dari antarmuka aplikasi.

Tema bawaan: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Setiap tema memuat palet terang dan gelap.

Menu mode dokumen menyediakan:

- **Terang/Gelap Otomatis** — mengikuti pengaturan `prefers-color-scheme` peramban
- **Selalu Gelap**
- **Selalu Terang**

CSS yang dihasilkan sama untuk pratinjau langsung dan HTML yang diunduh, sehingga dokumen yang diekspor sesuai dengan tema dan perilaku mode yang dipilih.

## Penyorotan Sintaksis

Blok kode berpagar disorot sintaksisnya bila pagarnya menyebutkan sebuah bahasa:

    ```python
    print("hello")
    ```

Penyorotan ditenagai oleh Highlight.js 11.9.0.

Bahasa yang didukung: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML, dan YAML.

## HTML Mentah

HTML mentah di dalam Markdown dinonaktifkan secara bawaan.

Ketika **Aktifkan HTML mentah** dinyalakan, aplikasi tetap membersihkan hasil render sebelum menampilkan atau mengekspornya. Pembersih akan menghapus atau membatasi konten yang berpotensi berbahaya, seperti:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formulir
- atribut penangan peristiwa seperti `onclick`
- URL `javascript:`
- konten tersemat tidak aman lainnya

Aktifkan HTML mentah hanya untuk Markdown yang Anda percayai.

Pratinjau hasil render juga diisolasi di dalam iframe bermode sandbox.

## Perender Markdown

Versi saat ini menyematkan **Marked 4.0.19** langsung di dalam berkas HTML agar aplikasi dapat bekerja secara luring.

Kode aplikasi menempatkan perender Markdown di balik lapisan adaptor kecil, sehingga pengurai yang disematkan dapat diganti tanpa merancang ulang bagian aplikasi lainnya.

Sasaran desain awalnya adalah `markdown-it`; versi saat ini menggunakan bundel peramban Marked yang tersedia saat pembuatan.

## Bahasa

Antarmuka mencakup:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Aplikasi otomatis memilih bahasa yang didukung berdasarkan lokal peramban dan mendukung tata letak RTL bila diperlukan.
