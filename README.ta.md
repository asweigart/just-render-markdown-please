# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

நேரடி HTML முன்னோட்டத்துடன் கூடிய, தனிப்பட்ட, இணையம் இல்லாமலும் இயங்கும் Markdown திருத்தி. **Just Render the Markdown, Please** ஒரே கோப்பில் அமைந்த வலைப் பயன்பாடு: HTML கோப்பைச் சேமித்து, உலாவியில் திறந்து, கணக்கு, சேவையகம், நிறுவல் அல்லது இணைய இணைப்பு இல்லாமல் பயன்படுத்தலாம். எல்லாத் தரவும் உங்கள் கணினியிலேயே இருக்கும்; எதுவும் பதிவேற்றப்படுவதில்லை.

[பயன்பாட்டைத் திற](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

தற்போதைய பதிப்பு: **0.2.0** — பயன்பாட்டின் "பற்றி" உரையாடலில் காட்டப்படுகிறது.

## அம்சங்கள்

- Markdown-இலிருந்து HTML-க்கான நேரடி முன்னோட்டம்
- கணினியில் பிரிந்த காட்சி: இடதுபுறம் Markdown திருத்தி, வலதுபுறம் வழங்கப்பட்ட HTML
- வழங்கப்பட்ட ஆவணத்தை முழுமையான, தன்னிறைவான `.html` கோப்பாகப் பதிவிறக்கலாம்
- உள்ளமைந்த ஆறு Markdown எடுத்துக்காட்டுகள்
- அட்டவணைகள், பணிப்பட்டியல்கள், அடித்தல் உரை, தானியங்கி இணைப்புகள், வேலிக் குறியீட்டுத் தொகுதிகள் உள்ளிட்ட GitHub பாணி Markdown அம்சங்கள்
- வேலிக் குறியீட்டுத் தொகுதிகளில் 36 மொழிகளுக்கான தொடரியல் சிறப்பொளியூட்டல் — திருத்தியிலும் வழங்கப்பட்ட ஆவணத்திலும்
- பாதுகாப்புக்காக மூல HTML இயல்பாகவே முடக்கப்பட்டுள்ளது
- 40 மொழிகளில் பயனர் இடைமுகம்
- விளம்பரங்கள், பதிவு, சந்தாக்கள், கண்காணிப்பான்கள் எதுவும் இல்லை

## ஆவணத் தோற்றங்கள்

வழங்கப்பட்ட Markdown ஆவணத்திற்குப் பயன்பாட்டு இடைமுகத்திலிருந்து தனியான, தனக்கே உரிய தோற்ற அமைப்பு உள்ளது.

உள்ளடங்கிய தோற்றங்கள்: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

ஒவ்வொரு தோற்றத்திலும் வெளிச்ச மற்றும் இருள் வண்ணத்தட்டுகள் இரண்டும் உள்ளன.

ஆவண முறை பட்டியல் வழங்குவது:

- **தானியங்கி வெளிச்சம்/இருள்** — உலாவியின் `prefers-color-scheme` அமைப்பைப் பின்பற்றுகிறது
- **எப்போதும் இருள்**
- **எப்போதும் வெளிச்சம்**

நேரடி முன்னோட்டத்திற்கும் பதிவிறக்கிய HTML-க்கும் ஒரே உருவாக்கப்பட்ட CSS பயன்படுத்தப்படுகிறது; எனவே ஏற்றுமதி செய்யப்பட்ட ஆவணங்கள் தேர்ந்தெடுத்த தோற்றத்துடனும் முறை நடத்தையுடனும் பொருந்துகின்றன.

## தொடரியல் சிறப்பொளியூட்டல்

வேலியில் மொழியின் பெயர் குறிப்பிடப்பட்டால், குறியீட்டுத் தொகுதிகள் தொடரியல் அடிப்படையில் சிறப்பொளியூட்டப்படும்:

    ```python
    print("hello")
    ```

சிறப்பொளியூட்டலை Highlight.js 11.9.0 இயக்குகிறது.

ஆதரிக்கப்படும் மொழிகள்: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML மற்றும் YAML.

## மூல HTML

Markdown-இல் உள்ள மூல HTML இயல்பாகவே முடக்கப்பட்டுள்ளது.

**மூல HTML-ஐ இயக்கு** என்பதை ஆன் செய்தாலும், காட்டுவதற்கு அல்லது ஏற்றுமதி செய்வதற்கு முன் பயன்பாடு வழங்கப்பட்ட முடிவைச் சுத்தப்படுத்துகிறது. ஆபத்தாக இருக்கக்கூடிய உள்ளடக்கத்தைச் சுத்திகரிப்பான் நீக்குகிறது அல்லது கட்டுப்படுத்துகிறது; எடுத்துக்காட்டாக:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- படிவங்கள்
- `onclick` போன்ற நிகழ்வுக் கையாளும் பண்புக்கூறுகள்
- `javascript:` முகவரிகள்
- பிற பாதுகாப்பற்ற உட்பொதிக்கப்பட்ட உள்ளடக்கம்

நீங்கள் நம்பும் Markdown-க்கு மட்டுமே மூல HTML-ஐ இயக்குங்கள்.

வழங்கப்பட்ட முன்னோட்டம், மணல்பெட்டி முறையிலான iframe-க்குள்ளும் தனிமைப்படுத்தப்படுகிறது.

## Markdown வழங்கி

தற்போதைய கட்டமைப்பு, பயன்பாடு இணையம் இல்லாமல் இயங்கும் வகையில் **Marked 4.0.19**-ஐ நேரடியாக HTML கோப்பில் உட்பொதிக்கிறது.

பயன்பாட்டுக் குறியீடு Markdown வழங்கியை ஒரு சிறிய இணைப்பான் அடுக்குக்குப் பின்னால் வைத்திருப்பதால், பயன்பாட்டின் மற்ற பகுதிகளை மறுவடிவமைக்காமலேயே உட்பொதிக்கப்பட்ட பாகுபடுத்தியை மாற்ற முடியும்.

முதலில் வடிவமைப்பு இலக்காக இருந்தது `markdown-it`; தற்போதைய கட்டமைப்பு, உருவாக்கும் நேரத்தில் கிடைத்த Marked உலாவித் தொகுப்பைப் பயன்படுத்துகிறது.

## மொழிகள்

இடைமுகத்தில் உள்ள மொழிகள்:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

உலாவியின் அமைவிடத்தின் அடிப்படையில் ஆதரிக்கப்படும் மொழியைப் பயன்பாடு தானாகவே தேர்ந்தெடுக்கிறது; தேவைப்படும் இடங்களில் வலமிருந்து இடம் தளவமைப்பையும் ஆதரிக்கிறது.
