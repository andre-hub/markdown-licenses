# Markdown Licenses

[🇬🇧 English Version](README.md)

Eine kuratierte Sammlung von Open-Source- und Open-Content-Lizenzen in sauberem, standardkonformem Markdown — direkt einsatzbereit als `LICENSE.md` in jedem Repository.

Alle Dateien verwenden Standard-ASCII-Anführungszeichen, UTF-8-Zeichenkodierung und kanonische [SPDX-Identifikatoren](https://spdx.org/licenses/) für zuverlässige Kompatibilität mit automatisierten Prüfwerkzeugen (REUSE, ScanCode, GitHub).

---

## Lizenzkategorien & Leitfaden zur Auswahl

Lizenzen unterscheiden sich maßgeblich darin, welche Freiheiten sie gewähren und welche Bedingungen sie an die Weitergabe oder Modifikation von Quellcode und Binärdateien knüpfen.

### 1. Permissiv (Freizügig)
* **Merkmale:** Minimale Einschränkungen. Gestattet die Nutzung, Modifikation und Weitergabe des Codes — auch in geschlossener oder kommerzieller Software. In der Regel muss lediglich der ursprüngliche Urheberrechtshinweis und der Haftungsausschluss beibehalten werden.
* **Typische Vertreter:**
  * **MIT:** Der globale De-facto-Standard — extrem kurz, verständlich und mit maximaler Akzeptanz in allen Ökosystemen.
  * **Apache 2.0:** Ausdrückliche Gewährung von Patentrechten und Schutz von Markenzeichen; ideal für größere Projekte und Zusammenarbeit mit Unternehmen.
  * **BSD 3-Clause / BSD 2-Clause:** Bewährte BSD-Varianten, wahlweise mit oder ohne explizitem Werbeverbot (Non-Endorsement-Klausel).
  * **0BSD / Boost 1.0 (BSL-1.0):** Befreien kompilierte Binärdistributionen von der Namensnennungspflicht.
  * **Blue Oak 1.0:** Eine moderne, in einfacher Sprache verfasste freizügige Lizenz.

### 2. Public Domain & Gemeinfreiheits-Fallbacks
* **Merkmale:** Verzicht auf alle Urheber- und Leistungsschutzrechte soweit gesetzlich zulässig. Beinhaltet eine weltweite, bedingungslose Ersatzlizenz für Rechtsordnungen, in denen ein vollständiger Urheberrechtsverzicht nicht möglich ist.
* **Typische Vertreter:**
  * **CC0 1.0:** Universeller Verzicht auf alle Rechte; Standard für offene Daten, Prompt-Sammlungen und Medien.
  * **The Unlicense:** Speziell auf Quellcode und Software ausgerichtete Gemeinfreiheits-Erklärung.

### 3. Copyleft auf Dateiebene / Bibliotheken (Schwaches Copyleft)
* **Merkmale:** Modifikationen an den lizenzierten Dateien bzw. der Bibliothek selbst müssen unter derselben Lizenz quelloffen bleiben. Das übergeordnete Anwendungsprojekt bzw. der eigene Anwendungscode darf jedoch unter einer beliebigen (auch proprietären) Lizenz verbleiben.
* **Typische Vertreter:**
  * **MPL 2.0 (Mozilla Public License):** Pragmatisches, dateibasiertes Copyleft; sehr unternehmensfreundlich.
  * **LGPL 3.0 / LGPL 2.1:** Standard für geteilte Bibliotheken; dynamisches Verlinken überträgt das Copyleft nicht auf die Hauptanwendung.
  * **EPL 2.0 (Eclipse Public License):** Beliebt im Java- und Enterprise-Ökosystem mit Regeln zur sekundären Lizenzkompatibilität.
  * **EUPL 1.2:** Zugeschnitten auf die europäische öffentliche Verwaltung; rechtlich gleichwertig verbindlich in 23 Amtssprachen der EU.

### 4. Starkes Copyleft
* **Merkmale:** Jedes abgeleitete oder fest verknüpfte Werk muss bei der Weitergabe vollständig unter denselben Lizenzbedingungen offengelegt werden. Garantiert, dass Verbesserungen und Erweiterungen dauerhaft für die Allgemeinheit frei bleiben ("Virale Wirkung").
* **Typische Vertreter:**
  * **GPL 3.0:** Umfassendes starkes Copyleft inklusive Patentklauseln und Schutz gegen Tivoisierung (Hardwaresperren gegen modifizierten Code).
  * **GPL 2.0:** Bewährter historischer Standard (u. a. im Linux-Kernel); verlangt Quellcode-Herausgabe bei Binärweitergabe.

### 5. Netzwerk- / SaaS-Copyleft
* **Merkmale:** Schließt das sogenannte "ASP-/SaaS-Schlupfloch". Verlangt die Offenlegung des Quellcodes auch dann, wenn die Software nicht als Binärdatei verteilt, sondern als Dienst über ein Netzwerk (Cloud, Web-App) bereitgestellt wird.
* **Typische Vertreter:**
  * **AGPL 3.0 (Affero GPL):** Der Goldstandard für Web-Backends, Cloud-Dienste und netzwerkfähige Software, die vor geschlossenen Cloud-Adaptionen geschützt werden sollen.

### 6. Dokumentation, Medien & Daten
* **Merkmale:** Speziell für kreative Werke, Handbücher, Spezifikationen und Datenbanken konzipiert, für die Softwarelizenzen rechtlich unpassend sind.
* **Typische Vertreter:**
  * **CC-BY 4.0:** Freizügig für Dokumentation, Blogs und Lernmaterialien (Namensnennung erforderlich).
  * **CC-BY-SA 4.0:** Copyleft (Share-Alike) für Wikis, Bücher und kooperative Inhalte.
  * **ODbL 1.0:** Copyleft speziell für strukturierte Datenbestände und Datenbanken (z. B. OpenStreetMap).

---

## Welche Lizenz für welchen Zweck?

| Dein Ziel | Empfohlene Lizenz | Warum? |
| :--- | :--- | :--- |
| **Maximale Reichweite, minimale Hürden** | [MIT](mit.md) | Standard für Open Source; erlaubt auch Einbindung in kommerzielle Produkte. |
| **Unternehmensprojekt mit Patentschutz** | [Apache-2.0](apache-2.0.md) | Beinhaltet explizite Patentrechte und schützt Projekt-Markennamen. |
| **C/C++-Bibliothek ohne Binär-Attribution** | [Boost 1.0](boost-1.0.md) / [0BSD](0bsd.md) | Nutzer müssen deinen Copyright-Hinweis nicht zwingend in Binärdateien einblenden. |
| **Bedingungslose Gemeinfreiheit** | [CC0 1.0](cc0-1.0.md) / [The Unlicense](unlicense.md) | Völliger Verzicht auf Rechte; maximal offene Bereitstellung. |
| **Bibliothek / Framework (offen halten, aber proprietär nutzbar)** | [MPL-2.0](mpl-2.0.md) oder [LGPL-3.0](lgpl-3.0.md) | Änderungen an der Bibliothek bleiben frei; die anbindende App bleibt geschützt. |
| **Behörden- und EU-Kontext** | [EUPL-1.2](eupl-1.2.md) | Speziell für europäische Rechtsprechung mit 23 amtlichen Sprachfassungen. |
| **Vollständiger Schutz vor Kommerzialisierung (Desktop/CLI)** | [GPL-3.0](gpl-3.0.md) | Alle Weiterentwicklungen müssen zwingend Open Source bleiben. |
| **Webdienst / Cloud-Software (SaaS-Schutz)** | [AGPL-3.0](agpl-3.0.md) | Verhindert, dass Dritte den Code als Cloud-Dienst nutzen, ohne eigene Änderungen offenzulegen. |
| **Dokumentation, Texte, Medien** | [CC-BY-4.0](cc-by-4.0.md) / [CC-BY-SA-4.0](cc-by-sa-4.0.md) | Zugeschnitten auf Text- und Mediengüter (permissiv oder mit Share-Alike). |
| **Offene Datenbanken & Geodaten** | [ODbL-1.0](odbl-1.0.md) | Schützt Datenintegrität und Rechte an strukturierten Datenbanken. |

---

## Schnellübersicht (Aktive Lizenzen)

| Lizenz | SPDX-ID | Datei | Kategorie / Kurzbeschreibung |
| :--- | :--- | :--- | :--- |
| **MIT** | `MIT` | [`mit.md`](mit.md) | Permissiv, kurz, maximal verbreitet |
| **Apache 2.0** | `Apache-2.0` | [`apache-2.0.md`](apache-2.0.md) | Permissiv mit ausdrücklicher Patent- & Markengewährung |
| **BSD 3-Clause** | `BSD-3-Clause` | [`bsd-3-clause.md`](bsd-3-clause.md) | Permissiv mit Werbeverbotsklausel (Non-Endorsement) |
| **BSD 2-Clause** | `BSD-2-Clause` | [`bsd-2-clause.md`](bsd-2-clause.md) | Vereinfachte freizügige Lizenz ohne Werbeklausel |
| **0BSD** | `0BSD` | [`0bsd.md`](0bsd.md) | Null-Klausel-Lizenz, keine Namensnennung in Binärdateien |
| **ISC** | `ISC` | [`isc.md`](isc.md) | Funktional äquivalent zu BSD 2-Clause / MIT, kompakte Formulierung |
| **Boost 1.0** | `BSL-1.0` | [`boost-1.0.md`](boost-1.0.md) | Permissiv, befreit Binärdistributionen von Namensnennung |
| **Blue Oak 1.0** | `BlueOak-1.0.0` | [`blueoak-1.0.0.md`](blueoak-1.0.0.md) | Moderne, verständlich formulierte freizügige Lizenz |
| **CC0 1.0** | `CC0-1.0` | [`cc0-1.0.md`](cc0-1.0.md) | Gemeinfreiheits-Erklärung (Public Domain) & weltweiter Fallback |
| **The Unlicense** | `Unlicense` | [`unlicense.md`](unlicense.md) | Gemeinfreiheits-Erklärung speziell für Software |
| **MPL 2.0** | `MPL-2.0` | [`mpl-2.0.md`](mpl-2.0.md) | Schwaches Copyleft (Dateiebene), unternehmensfreundlich |
| **LGPL 3.0** | `LGPL-3.0-or-later` | [`lgpl-3.0.md`](lgpl-3.0.md) | Schwaches Copyleft (dynamisches Verlinken erlaubt) |
| **LGPL 2.1** | `LGPL-2.1-or-later` | [`lgpl-2.1.md`](lgpl-2.1.md) | Traditionelles Bibliotheks-Copyleft (C/C++-Bibliotheken) |
| **EPL 2.0** | `EPL-2.0` | [`epl-2.0.md`](epl-2.0.md) | Schwaches Copyleft mit sekundärer Lizenzkompatibilität |
| **EUPL 1.2** | `EUPL-1.2` | [`eupl-1.2.md`](eupl-1.2.md) | Copyleft der Europäischen Union, 23 Amtssprachen |
| **GPL 3.0** | `GPL-3.0-or-later` | [`gpl-3.0.md`](gpl-3.0.md) | Starkes Copyleft mit Patentklausel & Schutz vor Tivoisierung |
| **GPL 2.0** | `GPL-2.0-only` | [`gpl-2.0.md`](gpl-2.0.md) | Starkes Copyleft (Linux-Kernel-Standard) |
| **AGPL 3.0** | `AGPL-3.0-or-later` | [`agpl-3.0.md`](agpl-3.0.md) | Starkes Netzwerk-/SaaS-Copyleft für Webdienste |
| **CC-BY 4.0** | `CC-BY-4.0` | [`cc-by-4.0.md`](cc-by-4.0.md) | Permissiv für Dokumentation, Daten & Medien |
| **CC-BY-SA 4.0** | `CC-BY-SA-4.0` | [`cc-by-sa-4.0.md`](cc-by-sa-4.0.md) | Copyleft für kreative Werke, Wikis & Dokumentation |
| **ODbL 1.0** | `ODbL-1.0` | [`odbl-1.0.md`](odbl-1.0.md) | Copyleft für strukturierte Daten & Datenbanken |

---

## Archivierte Lizenzen (`archive/`)

Veraltete, ersetzte oder historisch problematische Lizenzen (wie etwa Artistic 2.0, BSD 4-Clause mit Werbeklausel, CC-BY-SA 3.0, EPL 1.0, GFDL 1.3, GPL 1.0 oder MS-PL) werden im Verzeichnis [`archive/`](archive/README.md) aufbewahrt.

Sie stehen weiterhin für historische Recherchen und bestehende Altprojekte zur Verfügung, werden jedoch **für neue Projekte ausdrücklich nicht mehr empfohlen**. Eine detaillierte Übersicht über die Gründe und moderne Alternativen findet sich in [`archive/README.md`](archive/README.md).

---

## Verwendung in 3 Schritten

1. **Passende Lizenz wählen:** Wähle anhand der Projektziele und des Leitfadens oben die richtige Lizenz aus.
2. **Datei kopieren:** Kopiere die entsprechende `.md`-Datei als `LICENSE.md` (oder `LICENSE`) in das Wurzelverzeichnis deines Repositories.
3. **Platzhalter ausfüllen:** Ergänze die Platzhalter im Lizenztext (wie z. B. Copyright-Jahr `<year>` und Name des Urhebers/Rechteinhabers `<name of author / copyright holder>`).
