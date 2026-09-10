# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Un editor Markdown privato e offline con anteprima HTML in tempo reale. **Just Render the Markdown, Please** è un'applicazione web in un unico file: salva il file HTML, aprilo in un browser e usalo senza account, server, installazione o connessione a internet. Tutti i dati restano sul tuo computer; nulla viene caricato online.

[Apri l'applicazione](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Versione attuale: **0.2.0** — mostrata nella finestra "Informazioni" dell'app.

## Funzionalità

- Anteprima in tempo reale da Markdown a HTML
- Vista affiancata su desktop: editor Markdown a sinistra, HTML renderizzato a destra
- Download del documento renderizzato come file `.html` completo e autonomo
- Sei esempi Markdown integrati
- Funzionalità Markdown in stile GitHub, tra cui tabelle, elenchi di attività, testo barrato, collegamenti automatici e blocchi di codice delimitati
- Evidenziazione della sintassi per 36 linguaggi nei blocchi di codice delimitati, sia nell'editor sia nel documento renderizzato
- L'HTML grezzo è disattivato per impostazione predefinita, per sicurezza
- Interfaccia utente in 40 lingue
- Nessuna pubblicità, registrazione, abbonamento o tracker

## Temi del documento

Il documento Markdown renderizzato ha un proprio sistema di temi, indipendente dall'interfaccia dell'app.

Temi inclusi: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Ogni tema contiene sia una tavolozza chiara sia una scura.

Il menu a discesa della modalità documento offre:

- **Chiaro/Scuro automatico** — segue l'impostazione `prefers-color-scheme` del browser
- **Sempre scuro**
- **Sempre chiaro**

Lo stesso CSS generato viene usato sia per l'anteprima dal vivo sia per l'HTML scaricato, quindi i documenti esportati corrispondono al tema e al comportamento della modalità selezionati.

## Evidenziazione della sintassi

I blocchi di codice delimitati vengono evidenziati quando la delimitazione indica un linguaggio:

    ```python
    print("hello")
    ```

L'evidenziazione è fornita da Highlight.js 11.9.0.

Linguaggi supportati: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML e YAML.

## HTML grezzo

L'HTML grezzo nel Markdown è disattivato per impostazione predefinita.

Quando **Abilita HTML grezzo** è attivo, l'app continua comunque a sanificare il risultato renderizzato prima di mostrarlo o esportarlo. La sanificazione rimuove o limita contenuti potenzialmente pericolosi, come:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- moduli
- attributi gestori di eventi come `onclick`
- URL `javascript:`
- altri contenuti incorporati non sicuri

Abilita l'HTML grezzo solo per Markdown di cui ti fidi.

L'anteprima renderizzata è inoltre isolata in un iframe in modalità sandbox.

## Renderer Markdown

La build attuale incorpora **Marked 4.0.19** direttamente nel file HTML, così l'applicazione funziona offline.

Il codice dell'app mantiene il renderer Markdown dietro un piccolo livello di adattamento, il che permette di sostituire il parser incorporato senza riprogettare il resto dell'applicazione.

L'obiettivo di progetto originale era `markdown-it`; la build attuale usa il bundle browser di Marked disponibile durante la realizzazione.

## Lingue

L'interfaccia comprende:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

L'app seleziona automaticamente una lingua supportata in base alla localizzazione del browser e supporta il layout da destra a sinistra dove appropriato.
