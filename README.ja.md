# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

プライベートかつオフラインで使える、HTML ライブプレビュー付きの Markdown エディターです。**Just Render the Markdown, Please** は単一ファイルの Web アプリです。HTML ファイルを保存してブラウザーで開けば、アカウント・サーバー・インストール・インターネット接続なしで使えます。データはすべて自分のコンピューター内に留まり、何もアップロードされません。

[アプリを開く](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

現在のバージョン: **0.2.0** — アプリの「情報」ダイアログに表示されます。

## 機能

- Markdown から HTML へのライブプレビュー
- デスクトップの分割表示: 左に Markdown エディター、右にレンダリングされた HTML
- レンダリング結果を単体で完結する `.html` ファイルとしてダウンロード
- 6 種類の Markdown サンプルを内蔵
- 表、タスクリスト、打ち消し線、自動リンク、フェンス付きコードブロックなど、GitHub 風の Markdown 機能に対応
- フェンス付きコードブロックで 36 言語のシンタックスハイライトに対応（エディターとレンダリング結果の両方）
- 安全性のため、生の HTML は既定で無効
- 40 言語のユーザーインターフェイス
- 広告・登録・サブスクリプション・トラッカーは一切なし

## ドキュメントテーマ

レンダリングされた Markdown ドキュメントは、アプリの UI とは独立したテーマ機能を備えています。

同梱テーマ: Clean、GitHub、Book、Minimal、Terminal、Solarized、Monokai、Nord、Sepia、Large Print、Compact、Typewriter

どのテーマにもライトとダークの両方のパレットが含まれます。

ドキュメントモードのドロップダウンでは次を選べます。

- **自動ライト/ダーク** — ブラウザーの `prefers-color-scheme` 設定に従います
- **常にダーク**
- **常にライト**

ライブプレビューとダウンロードした HTML には同じ生成 CSS が使われるため、書き出したドキュメントは選択したテーマとモードの挙動どおりになります。

## シンタックスハイライト

フェンスに言語名を書くと、コードブロックがシンタックスハイライトされます。

    ```python
    print("hello")
    ```

ハイライトは Highlight.js 11.9.0 によるものです。

対応言語: Bash、C、C++、C#、CSS、Diff、Go、GraphQL、INI/TOML、Java、JavaScript、JSON、Kotlin、Less、Lua、Makefile、Markdown、Objective-C、Perl、PHP、PHP Template、Plain Text、Python、Python REPL、R、Ruby、Rust、SCSS、Shell Session、SQL、Swift、TypeScript、VB.NET、WebAssembly、XML/HTML、YAML。

## 生の HTML

Markdown 内の生の HTML は既定で無効です。

**生の HTML を有効にする**をオンにしても、アプリは表示・書き出しの前にレンダリング結果をサニタイズします。サニタイザーは、次のような危険になり得る内容を削除または制限します。

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- フォーム
- `onclick` などのイベントハンドラー属性
- `javascript:` の URL
- その他の安全でない埋め込みコンテンツ

生の HTML は、信頼できる Markdown に対してのみ有効にしてください。

レンダリングされたプレビューは、サンドボックス化された iframe 内に隔離されます。

## Markdown レンダラー

現在のビルドはオフラインで動作するよう、**Marked 4.0.19** を HTML ファイルに直接埋め込んでいます。

アプリのコードは Markdown レンダラーを小さなアダプター層の背後に置いているため、アプリの他の部分を設計し直すことなく、埋め込みパーサーを差し替えられます。

当初の設計目標は `markdown-it` でしたが、現在のビルドでは制作時に利用できた Marked のブラウザーバンドルを使用しています。

## 言語

インターフェイスの対応言語:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

アプリはブラウザーのロケールに基づいて対応言語を自動選択し、必要に応じて RTL レイアウトにも対応します。
