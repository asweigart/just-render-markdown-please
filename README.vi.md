# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Một trình soạn thảo Markdown riêng tư, hoạt động ngoại tuyến, kèm bản xem trước HTML trực tiếp. **Just Render the Markdown, Please** là một ứng dụng web chỉ gồm một tệp: lưu tệp HTML, mở trong trình duyệt và dùng ngay mà không cần tài khoản, máy chủ, cài đặt hay kết nối internet. Mọi dữ liệu đều nằm trên máy của bạn; không có gì được tải lên.

[Mở ứng dụng](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Phiên bản hiện tại: **0.2.0** — hiển thị trong hộp thoại "Giới thiệu" của ứng dụng.

## Tính năng

- Xem trước trực tiếp quá trình chuyển Markdown sang HTML
- Chế độ chia đôi trên máy tính: trình soạn thảo Markdown bên trái, HTML đã kết xuất bên phải
- Tải tài liệu đã kết xuất về dưới dạng tệp `.html` độc lập, hoàn chỉnh
- Sáu ví dụ Markdown tích hợp sẵn
- Các tính năng Markdown kiểu GitHub, gồm bảng, danh sách công việc, chữ gạch ngang, liên kết tự động và khối mã có rào
- Tô sáng cú pháp cho 36 ngôn ngữ trong các khối mã có rào, cả trong trình soạn thảo lẫn tài liệu đã kết xuất
- HTML thô bị tắt theo mặc định vì lý do an toàn
- Giao diện người dùng bằng 40 ngôn ngữ
- Không quảng cáo, không đăng ký, không thuê bao, không trình theo dõi

## Chủ đề tài liệu

Tài liệu Markdown đã kết xuất có hệ thống chủ đề riêng, độc lập với giao diện ứng dụng.

Chủ đề có sẵn: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Mỗi chủ đề đều có cả bảng màu sáng và tối.

Danh sách chế độ tài liệu cung cấp:

- **Tự động Sáng/Tối** — theo thiết lập `prefers-color-scheme` của trình duyệt
- **Luôn tối**
- **Luôn sáng**

Bản xem trước trực tiếp và tệp HTML tải về dùng chung một bộ CSS được tạo ra, nên tài liệu xuất ra khớp với chủ đề và hành vi chế độ đã chọn.

## Tô sáng cú pháp

Khối mã có rào được tô sáng cú pháp khi rào ghi rõ tên ngôn ngữ:

    ```python
    print("hello")
    ```

Việc tô sáng do Highlight.js 11.9.0 đảm nhiệm.

Ngôn ngữ được hỗ trợ: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML và YAML.

## HTML thô

HTML thô trong Markdown bị tắt theo mặc định.

Khi bật **Bật HTML thô**, ứng dụng vẫn làm sạch kết quả kết xuất trước khi hiển thị hoặc xuất ra. Bộ làm sạch loại bỏ hoặc hạn chế những nội dung có thể gây nguy hiểm, chẳng hạn:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- biểu mẫu
- các thuộc tính xử lý sự kiện như `onclick`
- URL dạng `javascript:`
- các nội dung nhúng không an toàn khác

Chỉ bật HTML thô cho Markdown mà bạn tin tưởng.

Bản xem trước đã kết xuất còn được cách ly bên trong một iframe chạy ở chế độ hộp cát.

## Bộ kết xuất Markdown

Bản dựng hiện tại nhúng **Marked 4.0.19** trực tiếp vào tệp HTML để ứng dụng hoạt động ngoại tuyến.

Mã của ứng dụng đặt bộ kết xuất Markdown sau một lớp bộ chuyển đổi nhỏ, nhờ đó có thể thay thế bộ phân tích được nhúng mà không phải thiết kế lại phần còn lại của ứng dụng.

Mục tiêu thiết kế ban đầu là `markdown-it`; bản dựng hiện tại dùng gói trình duyệt của Marked có sẵn vào thời điểm xây dựng.

## Ngôn ngữ

Giao diện gồm:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Ứng dụng tự động chọn một ngôn ngữ được hỗ trợ dựa trên ngôn ngữ vùng của trình duyệt và hỗ trợ bố cục phải-sang-trái khi thích hợp.
