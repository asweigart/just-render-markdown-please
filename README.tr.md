# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Canlı HTML önizlemesi sunan, gizliliğe saygılı ve çevrimdışı çalışan bir Markdown düzenleyici. **Just Render the Markdown, Please**, tek dosyalık bir web uygulamasıdır: HTML dosyasını kaydedin, tarayıcıda açın ve hesap, sunucu, kurulum ya da internet bağlantısı olmadan kullanın. Tüm veriler bilgisayarınızda kalır; hiçbir şey yüklenmez.

[Uygulamayı aç](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Geçerli sürüm: **0.2.0** — uygulamanın "Hakkında" penceresinde gösterilir.

## Özellikler

- Markdown'dan HTML'e canlı önizleme
- Masaüstünde bölünmüş görünüm: solda Markdown düzenleyici, sağda işlenmiş HTML
- İşlenmiş belgeyi eksiksiz ve bağımsız bir `.html` dosyası olarak indirme
- Yerleşik altı Markdown örneği
- Tablolar, görev listeleri, üstü çizili metin, otomatik bağlantılar ve çitli kod blokları dahil GitHub tarzı Markdown özellikleri
- Çitli kod bloklarında 36 dil için sözdizimi vurgulama; hem düzenleyicide hem işlenmiş belgede
- Güvenlik nedeniyle ham HTML varsayılan olarak kapalı
- 40 dilde kullanıcı arayüzü
- Reklam, kayıt, abonelik veya izleyici yok

## Belge Temaları

İşlenmiş Markdown belgesinin, uygulama arayüzünden bağımsız kendi tema sistemi vardır.

Dahil edilen temalar: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Her tema hem açık hem koyu bir renk paleti içerir.

Belge modu açılır menüsü şunları sunar:

- **Otomatik Açık/Koyu** — tarayıcının `prefers-color-scheme` ayarını izler
- **Her zaman koyu**
- **Her zaman açık**

Canlı önizleme ile indirilen HTML aynı üretilmiş CSS'i kullanır; böylece dışa aktarılan belgeler seçilen tema ve mod davranışıyla eşleşir.

## Sözdizimi Vurgulama

Çit satırında bir dil belirtildiğinde kod blokları sözdizimi vurgulaması alır:

    ```python
    print("hello")
    ```

Vurgulama Highlight.js 11.9.0 ile sağlanır.

Desteklenen diller: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML ve YAML.

## Ham HTML

Markdown içindeki ham HTML varsayılan olarak kapalıdır.

**Ham HTML'i etkinleştir** açıldığında bile uygulama, görüntülemeden veya dışa aktarmadan önce sonucu temizler. Temizleyici, tehlikeli olabilecek içerikleri kaldırır ya da sınırlar; örneğin:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formlar
- `onclick` gibi olay işleyici öznitelikleri
- `javascript:` adresleri
- diğer güvensiz gömülü içerikler

Ham HTML'i yalnızca güvendiğiniz Markdown için etkinleştirin.

İşlenmiş önizleme ayrıca korumalı alan (sandbox) modundaki bir iframe içinde yalıtılır.

## Markdown İşleyici

Geçerli sürüm, uygulamanın çevrimdışı çalışabilmesi için **Marked 4.0.19**'u doğrudan HTML dosyasına gömer.

Uygulama kodu, Markdown işleyiciyi küçük bir bağdaştırıcı katmanın arkasında tutar; böylece gömülü ayrıştırıcı, uygulamanın geri kalanı yeniden tasarlanmadan değiştirilebilir.

Özgün tasarım hedefi `markdown-it` idi; geçerli sürüm, oluşturma sırasında elde edilebilen Marked tarayıcı paketini kullanır.

## Diller

Arayüzde bulunan diller:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Uygulama, tarayıcı yerel ayarına göre desteklenen bir dili otomatik seçer ve uygun olduğunda sağdan sola düzeni destekler.
