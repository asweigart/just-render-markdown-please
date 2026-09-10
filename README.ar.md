# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

محرِّر Markdown خاص يعمل دون اتصال بالإنترنت مع معاينة HTML مباشرة. تطبيق **Just Render the Markdown, Please** هو تطبيق ويب من ملف واحد: احفظ ملف HTML، وافتحه في المتصفح، واستخدمه دون حساب أو خادم أو تثبيت أو اتصال بالإنترنت. تبقى جميع البيانات على جهازك ولا يُرفع أي شيء.

[فتح التطبيق](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

الإصدار الحالي: **0.2.0** — يظهر في نافذة «حول» داخل التطبيق.

## المزايا

- معاينة مباشرة لتحويل Markdown إلى HTML
- عرض مقسَّم على سطح المكتب: محرِّر Markdown على جهة والمخرجات المعروضة بصيغة HTML على الجهة الأخرى
- تنزيل المستند المعروض كملف `.html` مستقل وكامل
- ستة أمثلة Markdown مضمَّنة
- مزايا Markdown بأسلوب GitHub، وتشمل الجداول وقوائم المهام والنص المشطوب والروابط التلقائية وكتل التعليمات البرمجية المسوَّرة
- تمييز صياغي لست وثلاثين لغة برمجة داخل الكتل المسوَّرة، في المحرِّر وفي المستند المعروض معًا
- HTML الخام معطَّل افتراضيًا لأسباب أمنية
- واجهة استخدام بأربعين لغة
- بلا إعلانات ولا تسجيل ولا اشتراكات ولا أدوات تتبُّع

## سمات المستند

يملك مستند Markdown المعروض نظام سمات خاصًا به، مستقلًا عن واجهة التطبيق.

السمات المضمَّنة: Clean وGitHub وBook وMinimal وTerminal وSolarized وMonokai وNord وSepia وLarge Print وCompact وTypewriter

تحتوي كل سمة على لوحة ألوان فاتحة وأخرى داكنة.

توفّر قائمة وضع المستند المنسدلة:

- **فاتح/داكن تلقائي** — يتبع إعداد `prefers-color-scheme` في المتصفح
- **داكن دائمًا**
- **فاتح دائمًا**

يُستخدَم نفس CSS المُولَّد للمعاينة المباشرة ولملف HTML المُنزَّل، لذا تطابق المستندات المصدَّرة السمة ووضع العرض المختارَين.

## التمييز الصياغي

تُميَّز الكتل البرمجية المسوَّرة صياغيًا عندما يذكر السور اسم اللغة:

    ```python
    print("hello")
    ```

يعتمد التمييز على Highlight.js 11.9.0.

اللغات المدعومة: Bash وC وC++ وC# وCSS وDiff وGo وGraphQL وINI/TOML وJava وJavaScript وJSON وKotlin وLess وLua وMakefile وMarkdown وObjective-C وPerl وPHP وPHP Template وPlain Text وPython وPython REPL وR وRuby وRust وSCSS وShell Session وSQL وSwift وTypeScript وVB.NET وWebAssembly وXML/HTML وYAML.

## HTML الخام

HTML الخام داخل Markdown معطَّل افتراضيًا.

عند تفعيل **تمكين HTML الخام**، يواصل التطبيق تنقية الناتج المعروض قبل عرضه أو تصديره. تزيل أداة التنقية المحتوى الخطر المحتمل أو تقيّده، مثل:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- النماذج
- سمات معالِجات الأحداث مثل `onclick`
- روابط `javascript:`
- غير ذلك من المحتوى المضمَّن غير الآمن

فعِّل HTML الخام فقط لمحتوى Markdown تثق به.

كما تُعزَل المعاينة المعروضة داخل إطار `iframe` يعمل في بيئة معزولة.

## مُصيِّر Markdown

يضمّن الإصدار الحالي **Marked 4.0.19** مباشرةً داخل ملف HTML كي يعمل التطبيق دون اتصال.

تُبقي شفرة التطبيق مُصيِّر Markdown خلف طبقة مهايئة صغيرة، مما يتيح استبدال المحلِّل المضمَّن دون إعادة تصميم بقية التطبيق.

كان الهدف التصميمي الأصلي هو `markdown-it`؛ أما الإصدار الحالي فيستخدم حزمة Marked للمتصفح التي كانت متاحة أثناء الإنشاء.

## اللغات

تشمل الواجهة:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

يختار التطبيق تلقائيًا لغةً مدعومة بناءً على إعدادات المتصفح المحلية، ويدعم التخطيط من اليمين إلى اليسار عند الاقتضاء.
