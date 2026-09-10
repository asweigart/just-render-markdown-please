# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Um editor de Markdown privado e offline com pré-visualização de HTML em tempo real. O **Just Render the Markdown, Please** é uma aplicação web de ficheiro único: guarde o ficheiro HTML, abra-o num navegador e use-o sem conta, servidor, instalação ou ligação à internet. Todos os dados ficam no seu computador; nada é enviado.

[Ver a aplicação](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Versão atual: **0.2.0** — apresentada na janela "Acerca de" da aplicação.

## Funcionalidades

- Pré-visualização de Markdown para HTML em tempo real
- Vista dividida no computador: editor de Markdown à esquerda, HTML renderizado à direita
- Transferência do documento renderizado como um ficheiro `.html` autónomo e completo
- Seis exemplos de Markdown incorporados
- Funcionalidades de Markdown ao estilo GitHub, incluindo tabelas, listas de tarefas, texto rasurado, ligações automáticas e blocos de código delimitados
- Realce de sintaxe para 36 linguagens em blocos de código delimitados, tanto no editor como no documento renderizado
- O HTML sem processamento está desativado por predefinição, por segurança
- Interface de utilizador em 40 idiomas
- Sem anúncios, registo, subscrições ou rastreadores

## Temas do documento

O documento Markdown renderizado tem o seu próprio sistema de temas, independente da interface da aplicação.

Temas incluídos: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Cada tema contém uma paleta clara e uma escura.

O menu de modo do documento oferece:

- **Claro/Escuro automático** — segue a definição `prefers-color-scheme` do navegador
- **Sempre escuro**
- **Sempre claro**

O mesmo CSS gerado é usado na pré-visualização em tempo real e no HTML transferido, pelo que os documentos exportados correspondem ao tema e ao comportamento de modo selecionados.

## Realce de sintaxe

Os blocos de código delimitados recebem realce de sintaxe quando a delimitação indica uma linguagem:

    ```python
    print("hello")
    ```

O realce é fornecido pelo Highlight.js 11.9.0.

Linguagens suportadas: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML e YAML.

## HTML sem processamento

O HTML sem processamento dentro do Markdown está desativado por predefinição.

Quando **Ativar HTML sem processamento** é ligado, a aplicação continua a higienizar o resultado renderizado antes de o mostrar ou exportar. O higienizador remove ou restringe conteúdo potencialmente perigoso, como:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formulários
- atributos de tratamento de eventos, como `onclick`
- URLs `javascript:`
- outro conteúdo incorporado inseguro

Ative o HTML sem processamento apenas para Markdown em que confie.

A pré-visualização renderizada é ainda isolada dentro de um iframe em modo sandbox.

## Renderizador de Markdown

A versão atual incorpora o **Marked 4.0.19** diretamente no ficheiro HTML, para que a aplicação funcione offline.

O código da aplicação mantém o renderizador de Markdown por trás de uma pequena camada adaptadora, o que permite substituir o analisador incorporado sem redesenhar o resto da aplicação.

O objetivo de design original era o `markdown-it`; a versão atual usa o pacote de navegador do Marked disponível durante a construção.

## Idiomas

A interface inclui:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

A aplicação seleciona automaticamente um idioma suportado com base na localização do navegador e suporta esquema da direita para a esquerda quando aplicável.
