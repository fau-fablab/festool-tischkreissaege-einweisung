Festool Tischkreissäge CSC SYS 50 Einweisung
============================================

Einweisung des [FAU FabLab](https://fablab.fau.de) für die Akku-Tischkreissäge [Festool CSC SYS 50 EBI](https://www.festool.de/produkte/saegen/tischkreissaege/576820---csc-sys-50).

Dies ist ein inoffizielles Dokument des FAU FabLab und steht in keiner Verbindung zur Festool GmbH.
„Festool“ ist eine Marke der Festool GmbH und wird hier nur zur Bezeichnung des Produkts verwendet.

Inhalt
------

- Technische Daten, die wichtigsten Teile (eigene Skizze), Regeln und Sicherheit, Schutzausrüstung
- Schnitthöhe und Neigung über das Display, Längsschnitt mit Parallelanschlag, Querschnitt mit Schiebeschlitten
- Rückschlag, Verbote, Arbeiten nach dem Sägen, Infos für Betreuer:innen

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/festool-tischkreissaege-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/festool-tischkreissaege-einweisung/einweisung_Tischkreissaege.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/festool-tischkreissaege-einweisung/einweisungsliste_Tischkreissaege.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/festool-tischkreissaege-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Das gelbe Hinweisschild für die Säge steht im Repo [hinweisschilder](https://github.com/fau-fablab/hinweisschilder).

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/festool-tischkreissaege-einweisung.git
cd festool-tischkreissaege-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/festool-tischkreissaege-einweisung/status.svg)](https://brain.fablab.fau.de/build/festool-tischkreissaege-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/festool-tischkreissaege-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/festool-tischkreissaege-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/festool-tischkreissaege-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/festool-tischkreissaege-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

Die Einweisung ist selbst formuliert und enthält keine Texte oder Abbildungen aus der Festool-Betriebsanleitung.
Die Fotos in `bilder/` sind selbst fotografiert (siehe `bilder/QUELLEN.md`), die Nummern der Bauteile werden
per TikZ darübergelegt. Die Sicherheitszeichen (ISO 7010, gemeinfrei) kommen aus fablab-document.
**Beim Bearbeiten nichts aus der Festool-Anleitung übernehmen, auch nicht sinngemäß Satz für Satz.** Bilder bitte
selbst fotografieren oder nur mit freier, kompatibler Lizenz (z. B. CC BY-SA von Wikimedia Commons, mit Quellenangabe)
verwenden.
