# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

لائیو HTML پیش نظارہ کے ساتھ ایک نجی، آف لائن مارک ڈاؤن ایڈیٹر۔ **Just Render the Markdown, Please** ایک ہی فائل پر مشتمل ویب ایپ ہے: HTML فائل محفوظ کریں، براؤزر میں کھولیں، اور بغیر کسی اکاؤنٹ، سرور، انسٹالیشن یا انٹرنیٹ کنکشن کے استعمال کریں۔ تمام ڈیٹا آپ کے کمپیوٹر پر ہی رہتا ہے؛ کچھ بھی اپ لوڈ نہیں ہوتا۔

[ایپ کھولیں](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

موجودہ ورژن: **0.2.0** — ایپ کے "تعارف" ڈائیلاگ میں دکھایا جاتا ہے۔

## خصوصیات

- مارک ڈاؤن سے HTML کا لائیو پیش نظارہ
- ڈیسک ٹاپ پر منقسم منظر: ایک طرف مارک ڈاؤن ایڈیٹر، دوسری طرف رینڈر شدہ HTML
- رینڈر شدہ دستاویز کو مکمل، خود مختار `.html` فائل کے طور پر ڈاؤن لوڈ کریں
- چھ بلٹ اِن مارک ڈاؤن مثالیں
- GitHub طرز کی مارک ڈاؤن خصوصیات، بشمول جدولیں، کام کی فہرستیں، خط کشیدہ متن، خودکار لنکس اور فینسڈ کوڈ بلاکس
- فینسڈ کوڈ بلاکس میں 36 زبانوں کے لیے نحوی نمایاں سازی، ایڈیٹر اور رینڈر شدہ دستاویز دونوں میں
- حفاظت کی خاطر خام HTML بطور طے شدہ بند ہے
- 40 زبانوں میں صارف انٹرفیس
- کوئی اشتہار، رجسٹریشن، سبسکرپشن یا ٹریکر نہیں

## دستاویزی تھیمز

رینڈر شدہ مارک ڈاؤن دستاویز کا اپنا تھیم نظام ہے، جو ایپ کے انٹرفیس سے آزاد ہے۔

شامل تھیمز: Clean، GitHub، Book، Minimal، Terminal، Solarized، Monokai، Nord، Sepia، Large Print، Compact، Typewriter

ہر تھیم میں روشن اور تاریک، دونوں رنگ پٹیاں موجود ہیں۔

دستاویزی موڈ کی فہرست میں دستیاب ہے:

- **خودکار لائٹ/ڈارک** — براؤزر کی `prefers-color-scheme` ترتیب کی پیروی کرتا ہے
- **ہمیشہ ڈارک**
- **ہمیشہ لائٹ**

لائیو پیش نظارہ اور ڈاؤن لوڈ کردہ HTML، دونوں کے لیے وہی تیار شدہ CSS استعمال ہوتی ہے، اس لیے برآمد کردہ دستاویزات منتخب تھیم اور موڈ کے مطابق ہوتی ہیں۔

## نحوی نمایاں سازی

جب فینس میں زبان کا نام دیا جائے تو کوڈ بلاکس نحوی طور پر نمایاں کیے جاتے ہیں:

    ```python
    print("hello")
    ```

نمایاں سازی Highlight.js 11.9.0 کے ذریعے ہوتی ہے۔

معاون زبانیں: Bash، C، C++، C#، CSS، Diff، Go، GraphQL، INI/TOML، Java، JavaScript، JSON، Kotlin، Less، Lua، Makefile، Markdown، Objective-C، Perl، PHP، PHP Template، Plain Text، Python، Python REPL، R، Ruby، Rust، SCSS، Shell Session، SQL، Swift، TypeScript، VB.NET، WebAssembly، XML/HTML اور YAML۔

## خام HTML

مارک ڈاؤن میں خام HTML بطور طے شدہ بند ہے۔

جب **خام HTML فعال کریں** آن کیا جائے، تب بھی ایپ دکھانے یا برآمد کرنے سے پہلے رینڈر شدہ نتیجے کو صاف کرتی ہے۔ صفائی کا عمل ممکنہ طور پر خطرناک مواد کو ہٹا دیتا یا محدود کر دیتا ہے، جیسے:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- فارمز
- `onclick` جیسی ایونٹ ہینڈلر خصوصیات
- `javascript:` روابط
- دیگر غیر محفوظ سرایت شدہ مواد

خام HTML صرف اسی مارک ڈاؤن کے لیے فعال کریں جس پر آپ کو بھروسہ ہو۔

رینڈر شدہ پیش نظارہ سینڈ باکس شدہ iframe کے اندر بھی الگ رکھا جاتا ہے۔

## مارک ڈاؤن رینڈرر

موجودہ بلڈ **Marked 4.0.19** کو براہِ راست HTML فائل میں شامل کرتا ہے تاکہ ایپ آف لائن کام کرے۔

ایپ کا کوڈ مارک ڈاؤن رینڈرر کو ایک چھوٹی اڈاپٹر پرت کے پیچھے رکھتا ہے، جس سے باقی ایپ کو ازسرِ نو ڈیزائن کیے بغیر شامل شدہ پارسر بدلا جا سکتا ہے۔

ابتدائی ڈیزائن کا ہدف `markdown-it` تھا؛ موجودہ بلڈ تعمیر کے وقت دستیاب Marked براؤزر بنڈل استعمال کرتا ہے۔

## زبانیں

انٹرفیس میں شامل ہیں:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

ایپ براؤزر کے لوکیل کی بنیاد پر خودکار طور پر ایک معاون زبان منتخب کرتی ہے اور جہاں مناسب ہو وہاں دائیں سے بائیں ترتیب کی حمایت کرتی ہے۔
