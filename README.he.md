# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

עורך Markdown פרטי שפועל גם ללא חיבור לאינטרנט, עם תצוגה מקדימה חיה של HTML. ‏**Just Render the Markdown, Please** הוא יישום רשת בקובץ יחיד: שמרו את קובץ ה‑HTML, פתחו אותו בדפדפן והשתמשו בו בלי חשבון, שרת, התקנה או חיבור לאינטרנט. כל הנתונים נשארים במחשב שלכם; שום דבר אינו מועלה.

[פתיחת היישום](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

הגרסה הנוכחית: **0.2.0** — מוצגת בחלון "אודות" של היישום.

## תכונות

- תצוגה מקדימה חיה של המרת Markdown ל‑HTML
- תצוגה מפוצלת במחשב: עורך ה‑Markdown בצד אחד וה‑HTML המעובד בצד השני
- הורדת המסמך המעובד כקובץ `.html` שלם ועצמאי
- שש דוגמאות Markdown מובנות
- תכונות Markdown בסגנון GitHub, ובכללן טבלאות, רשימות משימות, טקסט מחוק, קישורים אוטומטיים ובלוקי קוד מגודרים
- הדגשת תחביר עבור 36 שפות בבלוקי קוד מגודרים, הן בעורך והן במסמך המעובד
- ‏HTML גולמי מושבת כברירת מחדל מטעמי אבטחה
- ממשק משתמש ב‑40 שפות
- ללא פרסומות, הרשמה, מנויים או רכיבי מעקב

## ערכות נושא למסמך

למסמך ה‑Markdown המעובד יש מערכת ערכות נושא משלו, נפרדת מממשק היישום.

ערכות הנושא הכלולות: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

כל ערכת נושא כוללת לוח צבעים בהיר ולוח צבעים כהה.

תפריט מצב המסמך מציע:

- **בהיר/כהה אוטומטי** — פועל לפי הגדרת `prefers-color-scheme` של הדפדפן
- **תמיד כהה**
- **תמיד בהיר**

אותו CSS נוצר משמש הן לתצוגה המקדימה החיה והן לקובץ ה‑HTML שמורידים, כך שמסמכים שמיוצאים תואמים לערכת הנושא ולהתנהגות המצב שנבחרו.

## הדגשת תחביר

בלוקי קוד מגודרים מודגשים תחבירית כאשר שורת הגדר מציינת שפה:

    ```python
    print("hello")
    ```

ההדגשה מופעלת באמצעות Highlight.js 11.9.0.

השפות הנתמכות: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML ו‑YAML.

## HTML גולמי

‏HTML גולמי בתוך Markdown מושבת כברירת מחדל.

כאשר האפשרות **הפעלת HTML גולמי** מופעלת, היישום עדיין מנקה את התוצאה המעובדת לפני הצגה או ייצוא. המנקה מסיר או מגביל תוכן שעלול להיות מסוכן, כגון:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- טפסים
- מאפייני מטפלי אירועים כמו `onclick`
- כתובות `javascript:`
- תוכן מוטמע לא בטוח אחר

הפעילו HTML גולמי רק עבור Markdown שאתם סומכים עליו.

התצוגה המקדימה המעובדת מבודדת גם בתוך iframe במצב ארגז חול.

## מנוע העיבוד של Markdown

הגרסה הנוכחית מטמיעה את **Marked 4.0.19** ישירות בקובץ ה‑HTML, כדי שהיישום יפעל ללא חיבור לאינטרנט.

קוד היישום מחזיק את מנוע העיבוד מאחורי שכבת מתאם קטנה, ולכן אפשר להחליף את המנתח המוטמע בלי לתכנן מחדש את שאר היישום.

יעד התכנון המקורי היה `markdown-it`; הגרסה הנוכחית משתמשת בחבילת הדפדפן של Marked שהייתה זמינה בזמן הבנייה.

## שפות

הממשק כולל:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

היישום בוחר אוטומטית שפה נתמכת לפי הגדרות האזור של הדפדפן, ותומך בפריסה מימין לשמאל היכן שנדרש.
