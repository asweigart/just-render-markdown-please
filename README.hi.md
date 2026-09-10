# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

लाइव HTML पूर्वावलोकन के साथ एक निजी, ऑफ़लाइन मार्कडाउन संपादक। **Just Render the Markdown, Please** एक ही फ़ाइल वाला वेब ऐप है: HTML फ़ाइल सहेजें, उसे ब्राउज़र में खोलें, और बिना खाते, सर्वर, इंस्टॉलेशन या इंटरनेट कनेक्शन के इसका उपयोग करें। सारा डेटा आपके कंप्यूटर पर ही रहता है; कुछ भी अपलोड नहीं होता।

[ऐप खोलें](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

वर्तमान संस्करण: **0.2.0** — ऐप के "परिचय" संवाद में दिखाया जाता है।

## विशेषताएँ

- मार्कडाउन से HTML का लाइव पूर्वावलोकन
- डेस्कटॉप पर विभाजित दृश्य: बाईं ओर मार्कडाउन संपादक, दाईं ओर रेंडर किया गया HTML
- रेंडर किए गए दस्तावेज़ को पूर्ण, स्वतंत्र `.html` फ़ाइल के रूप में डाउनलोड करें
- छह अंतर्निहित मार्कडाउन उदाहरण
- GitHub-शैली की मार्कडाउन सुविधाएँ, जिनमें तालिकाएँ, कार्य-सूचियाँ, काट कर लिखा पाठ, स्वतः लिंक और फ़ेंस्ड कोड ब्लॉक शामिल हैं
- फ़ेंस्ड कोड ब्लॉक में 36 भाषाओं के लिए सिंटैक्स हाइलाइटिंग — संपादक और रेंडर किए गए दस्तावेज़, दोनों में
- सुरक्षा के लिए रॉ HTML डिफ़ॉल्ट रूप से बंद रहता है
- 40 भाषाओं में उपयोगकर्ता इंटरफ़ेस
- कोई विज्ञापन, पंजीकरण, सदस्यता या ट्रैकर नहीं

## दस्तावेज़ थीम

रेंडर किए गए मार्कडाउन दस्तावेज़ की अपनी थीम प्रणाली है, जो ऐप के इंटरफ़ेस से स्वतंत्र है।

शामिल थीम: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

हर थीम में हल्का और गहरा, दोनों रंग-पटल होते हैं।

दस्तावेज़-मोड ड्रॉपडाउन में उपलब्ध हैं:

- **ऑटो लाइट/डार्क** — ब्राउज़र की `prefers-color-scheme` सेटिंग का अनुसरण करता है
- **हमेशा डार्क**
- **हमेशा लाइट**

लाइव पूर्वावलोकन और डाउनलोड किए गए HTML, दोनों के लिए वही उत्पन्न CSS उपयोग होता है, इसलिए निर्यात किए गए दस्तावेज़ चुनी गई थीम और मोड व्यवहार से मेल खाते हैं।

## सिंटैक्स हाइलाइटिंग

जब फ़ेंस में भाषा का नाम दिया जाता है, तो कोड ब्लॉक सिंटैक्स-हाइलाइट होते हैं:

    ```python
    print("hello")
    ```

हाइलाइटिंग Highlight.js 11.9.0 से संचालित है।

समर्थित भाषाएँ: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML और YAML।

## रॉ HTML

मार्कडाउन में रॉ HTML डिफ़ॉल्ट रूप से बंद रहता है।

जब **रॉ HTML सक्षम करें** चालू किया जाता है, तब भी ऐप प्रदर्शित या निर्यात करने से पहले रेंडर किए गए परिणाम को साफ़ करता है। सैनिटाइज़र संभावित रूप से ख़तरनाक सामग्री को हटाता या सीमित करता है, जैसे:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- फ़ॉर्म
- `onclick` जैसी इवेंट-हैंडलर विशेषताएँ
- `javascript:` URL
- अन्य असुरक्षित एम्बेडेड सामग्री

रॉ HTML केवल उसी मार्कडाउन के लिए सक्षम करें जिस पर आप भरोसा करते हैं।

रेंडर किया गया पूर्वावलोकन एक सैंडबॉक्स किए गए iframe के भीतर भी अलग रखा जाता है।

## मार्कडाउन रेंडरर

वर्तमान बिल्ड **Marked 4.0.19** को सीधे HTML फ़ाइल में एम्बेड करता है ताकि ऐप ऑफ़लाइन काम करे।

ऐप का कोड मार्कडाउन रेंडरर को एक छोटी अडैप्टर परत के पीछे रखता है, जिससे शेष ऐप को दोबारा डिज़ाइन किए बिना एम्बेडेड पार्सर बदला जा सकता है।

मूल डिज़ाइन लक्ष्य `markdown-it` था; वर्तमान बिल्ड निर्माण के समय उपलब्ध Marked ब्राउज़र बंडल का उपयोग करता है।

## भाषाएँ

इंटरफ़ेस में शामिल हैं:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

ऐप ब्राउज़र की लोकेल के आधार पर स्वतः एक समर्थित भाषा चुनता है और जहाँ उपयुक्त हो वहाँ RTL लेआउट का समर्थन करता है।
