# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

실시간 HTML 미리보기를 제공하는 개인용 오프라인 마크다운 편집기입니다. **Just Render the Markdown, Please**는 단일 파일 웹 앱입니다. HTML 파일을 저장하고 브라우저에서 열면 계정, 서버, 설치, 인터넷 연결 없이 사용할 수 있습니다. 모든 데이터는 사용자의 컴퓨터에만 남으며, 아무것도 업로드되지 않습니다.

[앱 열기](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

현재 버전: **0.2.0** — 앱의 "정보" 대화 상자에 표시됩니다.

## 기능

- 마크다운에서 HTML로의 실시간 미리보기
- 데스크톱 분할 보기: 왼쪽에 마크다운 편집기, 오른쪽에 렌더링된 HTML
- 렌더링된 문서를 완전한 단독 실행형 `.html` 파일로 다운로드
- 기본 제공 마크다운 예제 6종
- 표, 작업 목록, 취소선, 자동 링크, 펜스 코드 블록 등 GitHub 스타일 마크다운 기능
- 펜스 코드 블록에서 36개 언어의 구문 강조 지원(편집기와 렌더링된 문서 모두)
- 보안을 위해 원시 HTML은 기본적으로 비활성화
- 40개 언어의 사용자 인터페이스
- 광고, 가입, 구독, 트래커 없음

## 문서 테마

렌더링된 마크다운 문서는 앱 UI와는 별개의 자체 테마 시스템을 사용합니다.

기본 제공 테마: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

모든 테마에는 밝은 팔레트와 어두운 팔레트가 모두 포함됩니다.

문서 모드 드롭다운에서 선택할 수 있는 항목:

- **자동 라이트/다크** — 브라우저의 `prefers-color-scheme` 설정을 따릅니다
- **항상 다크**
- **항상 라이트**

실시간 미리보기와 다운로드한 HTML에 동일하게 생성된 CSS가 사용되므로, 내보낸 문서는 선택한 테마와 모드 동작과 일치합니다.

## 구문 강조

펜스에 언어 이름을 지정하면 코드 블록에 구문 강조가 적용됩니다.

    ```python
    print("hello")
    ```

구문 강조는 Highlight.js 11.9.0을 사용합니다.

지원 언어: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML, YAML.

## 원시 HTML

마크다운 안의 원시 HTML은 기본적으로 비활성화되어 있습니다.

**원시 HTML 활성화**를 켜더라도 앱은 표시하거나 내보내기 전에 렌더링 결과를 소독합니다. 소독기는 다음과 같이 위험할 수 있는 내용을 제거하거나 제한합니다.

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- 폼
- `onclick` 같은 이벤트 처리기 속성
- `javascript:` URL
- 그 밖의 안전하지 않은 삽입 콘텐츠

신뢰할 수 있는 마크다운에 대해서만 원시 HTML을 활성화하세요.

렌더링된 미리보기는 샌드박스로 격리된 iframe 안에서도 분리되어 실행됩니다.

## 마크다운 렌더러

현재 빌드는 앱이 오프라인에서 동작하도록 **Marked 4.0.19**를 HTML 파일에 직접 포함합니다.

앱 코드는 마크다운 렌더러를 작은 어댑터 계층 뒤에 두기 때문에, 앱의 나머지 부분을 다시 설계하지 않고도 내장 파서를 교체할 수 있습니다.

원래 설계 목표는 `markdown-it`이었으나, 현재 빌드는 제작 당시 사용할 수 있었던 Marked 브라우저 번들을 사용합니다.

## 언어

인터페이스가 지원하는 언어:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

앱은 브라우저 로캘에 따라 지원되는 언어를 자동으로 선택하며, 필요한 경우 RTL 레이아웃을 지원합니다.
