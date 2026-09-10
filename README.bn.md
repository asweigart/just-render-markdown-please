# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

লাইভ HTML প্রিভিউ সহ একটি ব্যক্তিগত, অফলাইন মার্কডাউন সম্পাদক। **Just Render the Markdown, Please** একটি একক-ফাইল ওয়েব অ্যাপ: HTML ফাইলটি সংরক্ষণ করুন, ব্রাউজারে খুলুন, এবং কোনো অ্যাকাউন্ট, সার্ভার, ইনস্টলেশন বা ইন্টারনেট সংযোগ ছাড়াই ব্যবহার করুন। সব তথ্য আপনার কম্পিউটারেই থাকে; কিছুই আপলোড হয় না।

[অ্যাপটি খুলুন](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

বর্তমান সংস্করণ: **0.2.0** — অ্যাপের "সম্পর্কে" ডায়ালগে দেখানো হয়।

## বৈশিষ্ট্য

- মার্কডাউন থেকে HTML-এর লাইভ প্রিভিউ
- ডেস্কটপে বিভক্ত দৃশ্য: বাঁয়ে মার্কডাউন সম্পাদক, ডানে রেন্ডার করা HTML
- রেন্ডার করা নথিটি সম্পূর্ণ স্বয়ংসম্পূর্ণ `.html` ফাইল হিসেবে ডাউনলোড করুন
- ছয়টি অন্তর্নির্মিত মার্কডাউন উদাহরণ
- GitHub-ধাঁচের মার্কডাউন সুবিধা, যেমন টেবিল, কাজের তালিকা, কাটা লেখা, স্বয়ংক্রিয় লিঙ্ক ও ফেন্সড কোড ব্লক
- ফেন্সড কোড ব্লকে ৩৬টি ভাষার সিনট্যাক্স হাইলাইটিং — সম্পাদক ও রেন্ডার করা নথি, উভয়েই
- নিরাপত্তার জন্য কাঁচা HTML ডিফল্টভাবে নিষ্ক্রিয়
- ৪০টি ভাষার ব্যবহারকারী ইন্টারফেস
- কোনো বিজ্ঞাপন, নিবন্ধন, সাবস্ক্রিপশন বা ট্র্যাকার নেই

## নথির থিম

রেন্ডার করা মার্কডাউন নথির নিজস্ব থিম ব্যবস্থা রয়েছে, যা অ্যাপের ইন্টারফেস থেকে স্বাধীন।

অন্তর্ভুক্ত থিম: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

প্রতিটি থিমে হালকা ও গাঢ়, দুই ধরনের রঙ-প্যালেট রয়েছে।

নথি-মোড ড্রপডাউনে পাওয়া যায়:

- **স্বয়ংক্রিয় লাইট/ডার্ক** — ব্রাউজারের `prefers-color-scheme` সেটিং অনুসরণ করে
- **সবসময় ডার্ক**
- **সবসময় লাইট**

লাইভ প্রিভিউ ও ডাউনলোড করা HTML-এ একই উৎপন্ন CSS ব্যবহৃত হয়, তাই রপ্তানি করা নথি নির্বাচিত থিম ও মোডের আচরণের সঙ্গে মিলে যায়।

## সিনট্যাক্স হাইলাইটিং

ফেন্সে ভাষার নাম দিলে কোড ব্লক সিনট্যাক্স-হাইলাইট হয়:

    ```python
    print("hello")
    ```

হাইলাইটিং চালায় Highlight.js 11.9.0।

সমর্থিত ভাষা: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML ও YAML।

## কাঁচা HTML

মার্কডাউনে কাঁচা HTML ডিফল্টভাবে নিষ্ক্রিয়।

**কাঁচা HTML সক্রিয় করুন** চালু করলেও অ্যাপ প্রদর্শন বা রপ্তানির আগে রেন্ডার করা ফলাফল পরিশোধন করে। পরিশোধক সম্ভাব্য বিপজ্জনক উপাদান সরিয়ে দেয় বা সীমিত করে, যেমন:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- ফর্ম
- `onclick`-এর মতো ইভেন্ট-হ্যান্ডলার অ্যাট্রিবিউট
- `javascript:` URL
- অন্যান্য অনিরাপদ এম্বেড করা উপাদান

কেবল বিশ্বাসযোগ্য মার্কডাউনের জন্যই কাঁচা HTML সক্রিয় করুন।

রেন্ডার করা প্রিভিউ একটি স্যান্ডবক্সড iframe-এর ভেতরেও পৃথক রাখা হয়।

## মার্কডাউন রেন্ডারার

বর্তমান বিল্ড **Marked 4.0.19** সরাসরি HTML ফাইলে যুক্ত করে, যাতে অ্যাপটি অফলাইনে কাজ করে।

অ্যাপের কোড মার্কডাউন রেন্ডারারকে একটি ছোট অ্যাডাপ্টার স্তরের পেছনে রাখে, ফলে বাকি অ্যাপ নতুন করে না সাজিয়েই এম্বেড করা পার্সার বদলানো যায়।

মূল নকশার লক্ষ্য ছিল `markdown-it`; বর্তমান বিল্ড নির্মাণের সময় উপলব্ধ Marked ব্রাউজার বান্ডল ব্যবহার করে।

## ভাষা

ইন্টারফেসে রয়েছে:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

অ্যাপটি ব্রাউজারের লোকেল অনুযায়ী স্বয়ংক্রিয়ভাবে একটি সমর্থিত ভাষা বেছে নেয় এবং প্রযোজ্য ক্ষেত্রে RTL বিন্যাস সমর্থন করে।
