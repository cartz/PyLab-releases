# PyLab

**Python starten, nicht einrichten.**

PyLab ist eine kleine Python-Umgebung für den Unterricht: Editor, Ausführen-Knopf, Ausgabe. Python 3.14 und die wichtigsten Pakete sind eingebaut – kein System-Python, kein PATH, keine Internetverbindung nötig.

> **Alpha.** PyLab wird derzeit an einer Schule erprobt. Funktionen und Dateiformate können sich noch ändern.

**[Downloads und Änderungshinweise →](https://github.com/cartz/PyLab-releases/releases)**

Dieses Repository stellt die Installationsdateien und die automatischen Updates bereit. Der Quellcode wird separat verwaltet.

## Was PyLab bietet

- **Ausführen mit einem Klick** – die Ausgabe steht direkt darunter, Eingaben mit `input()` inklusive.
- **Fehler auf Deutsch** – unter jeder Fehlermeldung ein Satz, woran es meistens liegt, und ein Sprung zur Zeile.
- **Zeile für Zeile** – ein Programm schrittweise ausführen und den Variablen dabei zusehen.
- **Notebooks lesen und ausprobieren** – Jupyter-Notebooks als Arbeitsblatt, das unverändert bleibt.
- **Klausurmodus** – Name eingeben, schreiben, abgeben; gespeichert wird von selbst.
- **Alles offline dabei** – numpy, pandas, matplotlib, pillow, requests, openpyxl, turtle und die ganze Standardbibliothek.

## Systemvoraussetzungen

- **Mac** mit Apple-Chip (M1 oder neuer)
- **Windows 11** (x64 oder ARM)

## Installation auf dem Mac

1. Unter **[Releases](https://github.com/cartz/PyLab-releases/releases)** die Datei `PyLab_<Fassung>_mac_aarch64.dmg` herunterladen.
2. Die DMG öffnen und PyLab in den Ordner **Programme** ziehen.
3. PyLab aus dem Programme-Ordner starten.

### Beim ersten Start

PyLab ist nicht von Apple notarisiert. macOS öffnet es deshalb beim ersten Start nicht. Einmalig freigeben:

1. In der Meldung auf **Fertig** klicken (nicht „In den Papierkorb legen“).
2. **Systemeinstellungen → Datenschutz & Sicherheit** öffnen und zum Abschnitt **Sicherheit** scrollen.
3. Neben dem Hinweis zu PyLab auf **Dennoch öffnen** klicken und bestätigen.

Danach startet PyLab normal, auch nach Updates.

## Installation unter Windows

| Datei | Wofür |
| --- | --- |
| `PyLab_<Fassung>_win_x64-setup.exe` | Einzelplatz (Intel/AMD); bekommt Updates |
| `PyLab_<Fassung>_win_arm64-setup.exe` | Einzelplatz mit ARM-Prozessor; bekommt Updates |
| `PyLab_<Fassung>_win_x64_de-DE.msi` | Softwareverteilung der Schule, stille Installation mit `msiexec /i … /qn` |
| `PyLab_<Fassung>_win_*_portable.zip` | Ausprobieren ohne Installation |

Die Pakete sind nicht signiert. Beim Start von Hand warnt Windows SmartScreen: **Weitere Informationen → Trotzdem ausführen**.

## Updates

PyLab sucht beim Start still nach einer neuen Fassung. Gibt es eine, erscheint oben in der Werkzeugleiste ein Knopf; ein Klick zeigt die Änderungen und installiert auf Wunsch. Während einer Klausur wird nicht gesucht. Jedes Update ist signiert; PyLab installiert nichts anderes.

Keine Updates suchen: per MSI installierte Fassungen (dort verteilt die Schule), die portable Fassung, und Rechner, auf denen die Schule es mit `"updates": false` in `pylab-vorgaben.json` neben dem Programm abschaltet.

## Prüfsummen

Zu jedem Release gehört `SHA256SUMS.txt` mit den Prüfsummen aller Dateien.
