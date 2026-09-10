# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Un editor de Markdown privado y sin conexión con vista previa HTML en vivo. **Just Render the Markdown, Please** es una aplicación web de un solo archivo: guarda el archivo HTML, ábrelo en un navegador y úsalo sin cuenta, servidor, instalación ni conexión a internet. Todos los datos permanecen en tu equipo; no se sube nada.

[Ver la aplicación](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Versión actual: **0.2.0** — se muestra en el diálogo «Acerca de» de la aplicación.

## Características

- Vista previa en vivo de Markdown a HTML
- Vista dividida en escritorio: el editor de Markdown a la izquierda y el HTML renderizado a la derecha
- Descarga del documento renderizado como un archivo `.html` autónomo y completo
- Seis ejemplos de Markdown integrados
- Funciones de Markdown al estilo de GitHub, incluidas tablas, listas de tareas, texto tachado, enlaces automáticos y bloques de código delimitados
- Resaltado de sintaxis para 36 lenguajes en los bloques de código delimitados, tanto en el editor como en el documento renderizado
- El HTML sin procesar está desactivado de forma predeterminada por seguridad
- Interfaz de usuario en 40 idiomas
- Sin anuncios, registro, suscripciones ni rastreadores

## Temas del documento

El documento Markdown renderizado tiene su propio sistema de temas, independiente de la interfaz de la aplicación.

Temas incluidos: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Cada tema incluye una paleta clara y una oscura.

El menú desplegable de modo del documento ofrece:

- **Claro/Oscuro automático**: sigue la preferencia `prefers-color-scheme` del navegador
- **Siempre oscuro**
- **Siempre claro**

Se usa el mismo CSS generado tanto para la vista previa en vivo como para el HTML descargado, de modo que los documentos exportados coinciden con el tema y el comportamiento de modo seleccionados.

## Resaltado de sintaxis

Los bloques de código delimitados se resaltan cuando la línea de apertura indica un lenguaje:

    ```python
    print("hello")
    ```

El resaltado funciona con Highlight.js 11.9.0.

Lenguajes admitidos: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML y YAML.

## HTML sin procesar

El HTML sin procesar dentro del Markdown está desactivado de forma predeterminada.

Cuando se activa **Activar HTML sin procesar**, la aplicación sigue depurando el resultado renderizado antes de mostrarlo o exportarlo. El depurador elimina o restringe contenido potencialmente peligroso, como:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- formularios
- atributos de manejadores de eventos como `onclick`
- URL `javascript:`
- otro contenido incrustado inseguro

Activa el HTML sin procesar solo para Markdown en el que confíes.

La vista previa renderizada también queda aislada dentro de un iframe en modo sandbox.

## Renderizador de Markdown

La versión actual incrusta **Marked 4.0.19** directamente en el archivo HTML para que la aplicación funcione sin conexión.

El código de la aplicación mantiene el renderizador de Markdown detrás de una pequeña capa adaptadora, lo que permite reemplazar el analizador incrustado sin rediseñar el resto de la aplicación.

El objetivo de diseño original era `markdown-it`; la versión actual usa el paquete de navegador de Marked disponible durante su construcción.

## Idiomas

La interfaz incluye:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

La aplicación selecciona automáticamente un idioma admitido según la configuración regional del navegador y admite el diseño de derecha a izquierda cuando corresponde.
