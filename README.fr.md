# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Un éditeur Markdown privé et hors ligne avec un aperçu HTML en direct. **Just Render the Markdown, Please** est une application web en un seul fichier : enregistrez le fichier HTML, ouvrez-le dans un navigateur et utilisez-le sans compte, sans serveur, sans installation ni connexion internet. Toutes les données restent sur votre ordinateur ; rien n'est téléversé.

[Ouvrir l'application](https://inventwithpython.com/justrendermarkdownplease/just-render-markdown-please.html)

Version actuelle : **0.2.0** — affichée dans la fenêtre « À propos » de l'application.

## Fonctionnalités

- Aperçu en direct de la conversion Markdown vers HTML
- Vue partagée sur ordinateur : éditeur Markdown à gauche, HTML rendu à droite
- Téléchargement du document rendu sous forme de fichier `.html` autonome et complet
- Six exemples Markdown intégrés
- Fonctionnalités Markdown de style GitHub : tableaux, listes de tâches, texte barré, liens automatiques et blocs de code délimités
- Coloration syntaxique de 36 langages dans les blocs de code délimités, aussi bien dans l'éditeur que dans le document rendu
- Le HTML brut est désactivé par défaut pour des raisons de sécurité
- Interface utilisateur en 40 langues
- Ni publicités, ni inscription, ni abonnements, ni traceurs

## Thèmes du document

Le document Markdown rendu possède son propre système de thèmes, indépendant de l'interface de l'application.

Thèmes inclus : Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Chaque thème contient une palette claire et une palette sombre.

Le menu déroulant du mode document propose :

- **Clair/Sombre auto** — suit le réglage `prefers-color-scheme` du navigateur
- **Toujours sombre**
- **Toujours clair**

Le même CSS généré est utilisé pour l'aperçu en direct et pour le HTML téléchargé : les documents exportés respectent donc le thème et le comportement de mode sélectionnés.

## Coloration syntaxique

Les blocs de code délimités sont colorés lorsque la clôture indique un langage :

    ```python
    print("hello")
    ```

La coloration est assurée par Highlight.js 11.9.0.

Langages pris en charge : Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML et YAML.

## HTML brut

Le HTML brut dans le Markdown est désactivé par défaut.

Lorsque **Activer le HTML brut** est activé, l'application assainit malgré tout le résultat rendu avant l'affichage ou l'export. L'assainisseur supprime ou restreint les contenus potentiellement dangereux, tels que :

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- les formulaires
- les attributs gestionnaires d'événements comme `onclick`
- les URL `javascript:`
- les autres contenus intégrés non sûrs

N'activez le HTML brut que pour du Markdown auquel vous faites confiance.

L'aperçu rendu est en outre isolé dans une iframe en mode bac à sable.

## Moteur de rendu Markdown

La version actuelle intègre **Marked 4.0.19** directement dans le fichier HTML afin que l'application fonctionne hors ligne.

Le code de l'application place le moteur de rendu Markdown derrière une petite couche d'adaptation, ce qui permet de remplacer l'analyseur intégré sans repenser le reste de l'application.

L'objectif de conception initial était `markdown-it` ; la version actuelle utilise le paquet navigateur de Marked disponible au moment de la construction.

## Langues

L'interface comprend :

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

L'application sélectionne automatiquement une langue prise en charge selon la locale du navigateur et prend en charge la mise en page de droite à gauche le cas échéant.
