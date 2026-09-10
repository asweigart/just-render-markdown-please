# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

โปรแกรมแก้ไข Markdown ที่เป็นส่วนตัวและใช้งานแบบออฟไลน์ พร้อมตัวอย่าง HTML แบบสด **Just Render the Markdown, Please** เป็นเว็บแอปไฟล์เดียว เพียงบันทึกไฟล์ HTML เปิดในเบราว์เซอร์ แล้วใช้งานได้เลยโดยไม่ต้องมีบัญชี เซิร์ฟเวอร์ การติดตั้ง หรือการเชื่อมต่ออินเทอร์เน็ต ข้อมูลทั้งหมดอยู่ในเครื่องของคุณ ไม่มีการอัปโหลดสิ่งใด

[เปิดแอป](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

เวอร์ชันปัจจุบัน: **0.2.0** — แสดงในกล่องโต้ตอบ "เกี่ยวกับ" ของแอป

## คุณสมบัติ

- ตัวอย่างการแปลง Markdown เป็น HTML แบบสด
- มุมมองแบ่งครึ่งบนเดสก์ท็อป: ตัวแก้ไข Markdown อยู่ซ้าย ส่วน HTML ที่เรนเดอร์แล้วอยู่ขวา
- ดาวน์โหลดเอกสารที่เรนเดอร์แล้วเป็นไฟล์ `.html` แบบสมบูรณ์ในตัว
- ตัวอย่าง Markdown ในตัวหกชุด
- คุณสมบัติ Markdown แบบ GitHub ได้แก่ ตาราง รายการงาน ข้อความขีดฆ่า ลิงก์อัตโนมัติ และบล็อกโค้ดแบบมีรั้ว
- เน้นไวยากรณ์สำหรับ 36 ภาษาในบล็อกโค้ดแบบมีรั้ว ทั้งในตัวแก้ไขและในเอกสารที่เรนเดอร์แล้ว
- ปิด HTML ดิบไว้เป็นค่าเริ่มต้นเพื่อความปลอดภัย
- ส่วนติดต่อผู้ใช้ 40 ภาษา
- ไม่มีโฆษณา การลงทะเบียน การสมัครสมาชิก หรือตัวติดตาม

## ธีมของเอกสาร

เอกสาร Markdown ที่เรนเดอร์แล้วมีระบบธีมของตัวเอง แยกจากส่วนติดต่อผู้ใช้ของแอป

ธีมที่มีให้: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

ทุกธีมมีทั้งชุดสีสว่างและชุดสีมืด

เมนูโหมดเอกสารมีตัวเลือก:

- **สว่าง/มืดอัตโนมัติ** — เป็นไปตามการตั้งค่า `prefers-color-scheme` ของเบราว์เซอร์
- **มืดเสมอ**
- **สว่างเสมอ**

ตัวอย่างแบบสดและไฟล์ HTML ที่ดาวน์โหลดใช้ CSS ชุดเดียวกันที่สร้างขึ้น เอกสารที่ส่งออกจึงตรงกับธีมและพฤติกรรมของโหมดที่เลือกไว้

## การเน้นไวยากรณ์

บล็อกโค้ดแบบมีรั้วจะถูกเน้นไวยากรณ์เมื่อระบุชื่อภาษาไว้ที่รั้ว:

    ```python
    print("hello")
    ```

การเน้นไวยากรณ์ทำงานด้วย Highlight.js 11.9.0

ภาษาที่รองรับ: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML และ YAML

## HTML ดิบ

HTML ดิบภายใน Markdown ถูกปิดไว้เป็นค่าเริ่มต้น

เมื่อเปิด **เปิดใช้ HTML ดิบ** แอปยังคงทำความสะอาดผลลัพธ์ที่เรนเดอร์ก่อนแสดงหรือส่งออก ตัวทำความสะอาดจะลบหรือจำกัดเนื้อหาที่อาจเป็นอันตราย เช่น

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- ฟอร์ม
- แอตทริบิวต์ตัวจัดการเหตุการณ์ เช่น `onclick`
- URL แบบ `javascript:`
- เนื้อหาฝังตัวที่ไม่ปลอดภัยอื่น ๆ

ควรเปิด HTML ดิบเฉพาะกับ Markdown ที่คุณไว้วางใจเท่านั้น

ตัวอย่างที่เรนเดอร์แล้วยังถูกแยกไว้ภายใน iframe แบบแซนด์บ็อกซ์อีกด้วย

## ตัวเรนเดอร์ Markdown

รุ่นปัจจุบันฝัง **Marked 4.0.19** ไว้ในไฟล์ HTML โดยตรง เพื่อให้แอปทำงานแบบออฟไลน์ได้

โค้ดของแอปวางตัวเรนเดอร์ Markdown ไว้หลังชั้นอะแดปเตอร์ขนาดเล็ก จึงเปลี่ยนตัวแยกวิเคราะห์ที่ฝังไว้ได้โดยไม่ต้องออกแบบส่วนอื่นของแอปใหม่

เป้าหมายการออกแบบเดิมคือ `markdown-it` ส่วนรุ่นปัจจุบันใช้ชุดโปรแกรม Marked สำหรับเบราว์เซอร์ที่มีอยู่ในช่วงที่สร้างขึ้น

## ภาษา

ส่วนติดต่อผู้ใช้ประกอบด้วย:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

แอปจะเลือกภาษาที่รองรับโดยอัตโนมัติตามภาษาท้องถิ่นของเบราว์เซอร์ และรองรับการจัดวางแบบขวาไปซ้ายเมื่อเหมาะสม
