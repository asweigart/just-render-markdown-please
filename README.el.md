# Just Render the Markdown, Please

<!-- LANGNAV -->
[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [العربية](README.ar.md) | [Bahasa Indonesia](README.id.md) | [Português](README.pt.md) | [Français](README.fr.md) | [日本語](README.ja.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [हिन्दी](README.hi.md) | [বাংলা](README.bn.md) | [اردو](README.ur.md) | [한국어](README.ko.md) | [Tiếng Việt](README.vi.md) | [Türkçe](README.tr.md) | [Italiano](README.it.md) | [Nederlands](README.nl.md) | [Polski](README.pl.md) | [ไทย](README.th.md) | [فارسی](README.fa.md) | [Українська](README.uk.md) | [Čeština](README.cs.md) | [Bahasa Melayu](README.ms.md) | [Română](README.ro.md) | [Ελληνικά](README.el.md) | [עברית](README.he.md) | [Svenska](README.sv.md) | [Filipino](README.fil.md) | [தமிழ்](README.ta.md) | [Magyar](README.hu.md) | [Dansk](README.da.md) | [Suomi](README.fi.md) | [Norsk bokmål](README.nb.md) | [Slovenčina](README.sk.md) | [Български](README.bg.md) | [Српски](README.sr.md) | [Hrvatski](README.hr.md) | [Slovenščina](README.sl.md) | [Català](README.ca.md)
<!-- /LANGNAV -->

Ένας ιδιωτικός επεξεργαστής Markdown που λειτουργεί εκτός σύνδεσης, με ζωντανή προεπισκόπηση HTML. Το **Just Render the Markdown, Please** είναι μια εφαρμογή ιστού ενός μόνο αρχείου: αποθηκεύστε το αρχείο HTML, ανοίξτε το σε ένα πρόγραμμα περιήγησης και χρησιμοποιήστε το χωρίς λογαριασμό, διακομιστή, εγκατάσταση ή σύνδεση στο διαδίκτυο. Όλα τα δεδομένα παραμένουν στον υπολογιστή σας· τίποτα δεν μεταφορτώνεται.

[Άνοιγμα εφαρμογής](https://inventwithpython.com/justrenderthemarkdownplease/just-render-the-markdown-please.html)

Τρέχουσα έκδοση: **0.2.0** — εμφανίζεται στο παράθυρο «Σχετικά» της εφαρμογής.

## Χαρακτηριστικά

- Ζωντανή προεπισκόπηση από Markdown σε HTML
- Χωριστή προβολή σε υπολογιστή: επεξεργαστής Markdown αριστερά, αποδοσμένο HTML δεξιά
- Λήψη του αποδοσμένου εγγράφου ως πλήρους, αυτόνομου αρχείου `.html`
- Έξι ενσωματωμένα παραδείγματα Markdown
- Δυνατότητες Markdown σε στυλ GitHub, όπως πίνακες, λίστες εργασιών, διαγραμμένο κείμενο, αυτόματους συνδέσμους και μπλοκ κώδικα με φράχτες
- Επισήμανση σύνταξης για 36 γλώσσες στα μπλοκ κώδικα, τόσο στον επεξεργαστή όσο και στο αποδοσμένο έγγραφο
- Ο ακατέργαστος κώδικας HTML είναι απενεργοποιημένος από προεπιλογή, για λόγους ασφάλειας
- Διεπαφή χρήστη σε 40 γλώσσες
- Χωρίς διαφημίσεις, εγγραφή, συνδρομές ή ιχνηλάτες

## Θέματα εγγράφου

Το αποδοσμένο έγγραφο Markdown έχει το δικό του σύστημα θεμάτων, ανεξάρτητο από τη διεπαφή της εφαρμογής.

Διαθέσιμα θέματα: Clean, GitHub, Book, Minimal, Terminal, Solarized, Monokai, Nord, Sepia, Large Print, Compact, Typewriter

Κάθε θέμα περιέχει τόσο φωτεινή όσο και σκοτεινή παλέτα.

Το αναπτυσσόμενο μενού λειτουργίας εγγράφου προσφέρει:

- **Αυτόματο Φωτεινό/Σκοτεινό** — ακολουθεί τη ρύθμιση `prefers-color-scheme` του προγράμματος περιήγησης
- **Πάντα σκοτεινό**
- **Πάντα φωτεινό**

Το ίδιο παραγόμενο CSS χρησιμοποιείται και για τη ζωντανή προεπισκόπηση και για το ληφθέν HTML, ώστε τα εξαγόμενα έγγραφα να ταιριάζουν με το επιλεγμένο θέμα και τη συμπεριφορά λειτουργίας.

## Επισήμανση σύνταξης

Τα μπλοκ κώδικα με φράχτες επισημαίνονται συντακτικά όταν ο φράχτης δηλώνει γλώσσα:

    ```python
    print("hello")
    ```

Η επισήμανση βασίζεται στο Highlight.js 11.9.0.

Υποστηριζόμενες γλώσσες: Bash, C, C++, C#, CSS, Diff, Go, GraphQL, INI/TOML, Java, JavaScript, JSON, Kotlin, Less, Lua, Makefile, Markdown, Objective-C, Perl, PHP, PHP Template, Plain Text, Python, Python REPL, R, Ruby, Rust, SCSS, Shell Session, SQL, Swift, TypeScript, VB.NET, WebAssembly, XML/HTML και YAML.

## Ακατέργαστο HTML

Ο ακατέργαστος κώδικας HTML μέσα στο Markdown είναι απενεργοποιημένος από προεπιλογή.

Όταν ενεργοποιηθεί η επιλογή **Ενεργοποίηση ακατέργαστου HTML**, η εφαρμογή εξακολουθεί να εξυγιαίνει το αποδοσμένο αποτέλεσμα πριν από την εμφάνιση ή την εξαγωγή. Ο εξυγιαντής αφαιρεί ή περιορίζει δυνητικά επικίνδυνο περιεχόμενο, όπως:

- `<script>`
- `<iframe>`
- `<object>`
- `<embed>`
- φόρμες
- χαρακτηριστικά χειρισμού συμβάντων, όπως το `onclick`
- διευθύνσεις `javascript:`
- άλλο μη ασφαλές ενσωματωμένο περιεχόμενο

Ενεργοποιήστε τον ακατέργαστο κώδικα HTML μόνο για Markdown που εμπιστεύεστε.

Η αποδοσμένη προεπισκόπηση απομονώνεται επιπλέον μέσα σε iframe με λειτουργία sandbox.

## Μηχανή απόδοσης Markdown

Η τρέχουσα έκδοση ενσωματώνει το **Marked 4.0.19** απευθείας στο αρχείο HTML, ώστε η εφαρμογή να λειτουργεί εκτός σύνδεσης.

Ο κώδικας της εφαρμογής κρατά τη μηχανή απόδοσης Markdown πίσω από ένα μικρό στρώμα προσαρμογής, κάτι που επιτρέπει την αντικατάσταση του ενσωματωμένου αναλυτή χωρίς επανασχεδίαση της υπόλοιπης εφαρμογής.

Ο αρχικός στόχος σχεδίασης ήταν το `markdown-it`· η τρέχουσα έκδοση χρησιμοποιεί το πακέτο του Marked για προγράμματα περιήγησης που ήταν διαθέσιμο κατά την κατασκευή.

## Γλώσσες

Η διεπαφή περιλαμβάνει:

English, 简体中文, Español, العربية, Bahasa Indonesia, Português, Français, 日本語, Русский, Deutsch, हिन्दी, বাংলা, اردو, 한국어, Tiếng Việt, Türkçe, Italiano, Nederlands, Polski, ไทย, فارسی, Українська, Čeština, Bahasa Melayu, Română, Ελληνικά, עברית, Svenska, Filipino, தமிழ், Magyar, Dansk, Suomi, Norsk bokmål, Slovenčina, Български, Српски, Hrvatski, Slovenščina, Català

Η εφαρμογή επιλέγει αυτόματα μια υποστηριζόμενη γλώσσα με βάση τις τοπικές ρυθμίσεις του προγράμματος περιήγησης και υποστηρίζει διάταξη από δεξιά προς τα αριστερά όπου χρειάζεται.
