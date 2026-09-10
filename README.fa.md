# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

یک ویرایشگر Markdown خصوصی و آفلاین با پیش‌نمایش زندهٔ HTML. **Just Render the Markdown, Please** یک برنامهٔ وب تک‌فایلی است: فایل HTML را ذخیره کنید، در مرورگر باز کنید و بدون حساب کاربری، سرور، نصب یا اتصال اینترنتی از آن استفاده کنید. تمام داده‌ها روی رایانهٔ خودتان می‌ماند و چیزی بارگذاری نمی‌شود.

[باز کردن برنامه](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

نسخهٔ کنونی: **0.2.0** — در پنجرهٔ «درباره» برنامه نمایش داده می‌شود.

## ویژگی‌ها

- پیش‌نمایش زندهٔ تبدیل Markdown به HTML
- نمای دوبخشی در رایانه: ویرایشگر Markdown در یک سو و HTML رندرشده در سوی دیگر
- دانلود سند رندرشده به‌صورت یک فایل `.html` کامل و مستقل
- شش نمونهٔ Markdown از پیش‌ساخته
- ویژگی‌های Markdown به سبک GitHub، شامل جدول‌ها، فهرست کارها، متن خط‌خورده، پیوندهای خودکار و بلوک‌های کد نرده‌ای
- برجسته‌سازی نحوی برای ۳۶ زبان در بلوک‌های کد نرده‌ای، هم در ویرایشگر و هم در سند رندرشده
- HTML خام به‌طور پیش‌فرض برای امنیت غیرفعال است
- رابط کاربری به ۴۰ زبان
- بدون تبلیغات، ثبت‌نام، اشتراک یا ردیاب

## پوسته‌های سند

سند Markdown رندرشده سامانهٔ پوستهٔ مستقل خود را دارد که از رابط کاربری برنامه جداست.

پوسته‌های موجود: Clean، GitHub، Book، Minimal، Terminal، Solarized، Monokai، Nord، Sepia، Large Print، Compact، Typewriter

هر پوسته هم پالت روشن و هم پالت تیره دارد.

فهرست کشویی حالت سند این گزینه‌ها را دارد:

- **روشن/تیره خودکار** — از تنظیم `prefers-color-scheme` مرورگر پیروی می‌کند
- **همیشه تیره**
- **همیشه روشن**

برای پیش‌نمایش زنده و HTML دانلودشده از یک CSS تولیدشدهٔ یکسان استفاده می‌شود، بنابراین سندهای صادرشده با پوسته و رفتار حالت انتخاب‌شده مطابقت دارند.

## برجسته‌سازی نحوی

هرگاه در خط نرده نام زبان ذکر شود، بلوک کد از نظر نحوی برجسته می‌شود:

    ```python
    print("hello")
    ```

برجسته‌سازی با Highlight.js 11.9.0 انجام می‌شود.

زبان‌های پشتیبانی‌شده: Bash، C، C++، C#، CSS، Diff، Go، GraphQL، INI/TOML، Java، JavaScript، JSON، Kotlin، Less، Lua، Makefile، Markdown، Objective-C، Perl، PHP، PHP Template، Plain Text، Python، Python REPL، R، Ruby، Rust، SCSS، Shell Session، SQL، Swift، TypeScript، VB.NET، WebAssembly، XML/HTML و YAML.

## HTML خام

HTML خام درون Markdown به‌طور پیش‌فرض غیرفعال است.

هنگامی که **فعال‌سازی HTML خام** روشن باشد، برنامه همچنان پیش از نمایش یا خروجی‌گرفتن، نتیجهٔ رندرشده را پالایش می‌کند. پالایشگر محتوای بالقوه خطرناک را حذف یا محدود می‌کند؛ مانند:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- فرم‌ها
- ویژگی‌های رویدادگردان مانند `onclick`
- نشانی‌های `javascript:`
- دیگر محتوای جاسازی‌شدهٔ ناامن

HTML خام را تنها برای Markdownی فعال کنید که به آن اعتماد دارید.

پیش‌نمایش رندرشده افزون بر این، درون یک iframe جعبه‌شنی جداسازی می‌شود.

## موتور رندر Markdown

نسخهٔ کنونی **Marked 4.0.19** را مستقیماً در فایل HTML جاسازی می‌کند تا برنامه آفلاین کار کند.

کد برنامه موتور رندر Markdown را پشت یک لایهٔ مبدل کوچک نگه می‌دارد و همین کار جایگزینی تجزیه‌گر جاسازی‌شده را بدون بازطراحی بقیهٔ برنامه ممکن می‌سازد.

هدف طراحی اولیه `markdown-it` بود؛ نسخهٔ کنونی از بستهٔ مرورگری Marked استفاده می‌کند که هنگام ساخت در دسترس بود.

## زبان‌ها

رابط کاربری شامل این زبان‌هاست:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

برنامه بر پایهٔ زبان محلی مرورگر به‌طور خودکار یکی از زبان‌های پشتیبانی‌شده را برمی‌گزیند و در جای مناسب از چیدمان راست‌به‌چپ پشتیبانی می‌کند.
