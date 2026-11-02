# README – Entwicklung neuer Micro-Contents für den OER.net FDM-Basiskurs

Dieses Repository enthält Templates für die Erstellung von OER zum Forschungsdatenmanagement (FDM) im Markdownformat (*.md) zur Verwendung als [LiaScript](https://liascript.github.io/).

---

## 1. Ziel und Zweck

Diese README beschreibt, wie mithilfe der Templates `template_I.md` und `template_A.md` neue, modular aufgebaute Lehr- und Lerninhalte (Micro-Contents bzw. EduBricks) für den OER.net FDM-Basiskurs entwickelt werden können.

Der Basiskurs orientiert sich an der [Lernzielmatrix zum Forschungsdatenmanagement (LZM-FDM)](https://zenodo.org/records/15025246).

Ziel ist die Entwicklung von Lerninhalten, die:

- jeweils ein konkretes Lernziel adressieren,
- fachliche Inhalte und didaktische Aktivitäten voneinander trennen,
- flexibel in unterschiedlichen Lehr- und Lernsettings einsetzbar sind,
- einzeln oder kombiniert nachgenutzt werden können,
- offen lizenziert und bearbeitbar sind.

Die Materialien werden in Markdown erstellt und können beispielsweise über GitHub verwaltet oder mit LiaScript für digitale Lernumgebungen aufbereitet werden.

---

## 2. Aufbau des Brick-Systems

Für jedes Lernziel sind zwei Arten von Bricks vorgesehen.

### 2.1 Input-Brick (I)

Der Input-Brick enthält die fachlichen Grundlagen, die zur Erreichung eines Lernziels benötigt werden.

Dazu gehören:

- Lernziel und LZM-ID
- vorausgesetzte und weiterführende Lernziele
- Definitionen und zentrale Begriffe
- fachliche Erläuterungen
- relevante Merkmale und Prinzipien
- Beispiele und Anwendungskontexte
- Quellenangaben und weiterführende Literatur
- Lizenzhinweise und Autor:innen

**Template:** `template_I.md`

### 2.2 Aktivitäts-Brick (A)

Ein Aktivitäts-Brick beschreibt die didaktische Umsetzung eines Lernziels für eine bestimmte Sozialform.

Vorgesehene Sozialformen sind:

- Plenum
- Gruppenarbeit
- Partner:innenarbeit
- Einzelarbeit

Ein Aktivitäts-Brick enthält:

- Lernziel und LZM-ID
- Verweis auf den zugehörigen Input-Brick
- Sozialform
- Name und Beschreibung der Methode
- didaktische Ziele
- Gruppengröße und Zeitbedarf
- Vorbereitungsaufwand
- Ablauf und Durchführung
- benötigte Materialien und Werkzeuge
- Hinweise zur Durchführung
- Methodenquellen und Lizenzangaben

**Template:** `template_A.md`

Innerhalb eines Aktivitäts-Bricks können mehrere didaktische Methoden für dieselbe Sozialform beschrieben werden.

---

## 3. Dateibenennung

Die Dateien werden nach folgendem Schema benannt:

`[LZM-ID]_[Stichwort-Inhalt]_[Vermittlungsform]_[Sozialform].md`

Dabei gilt:

| Bestandteil | Bedeutung |
|---|---|
| LZM-ID | Eindeutige Kennung aus der Lernzielmatrix |
| Stichwort-Inhalt | Kurze Beschreibung des Lerninhalts |
| I | Input |
| A | Aktivität/Aufgabe |
| Sozialform | Plenum, Gruppenarbeit, Partner:innenarbeit oder Einzelarbeit |

Bei Input-Bricks entfällt die Sozialform.

### Beispiel: Prinzipien von Open Science

Für das Lernziel `01_008_0136` ergeben sich folgende Dateien:

- `01_008_0136_Prinzipien-Open-Science_I.md`
- `01_008_0136_Prinzipien-Open-Science_A_Plenum.md`
- `01_008_0136_Prinzipien-Open-Science_A_Gruppenarbeit.md`
- `01_008_0136_Prinzipien-Open-Science_A_Partner:innenarbeit.md`
- `01_008_0136_Prinzipien-Open-Science_A_Einzelarbeit.md`

Die Benennung der Sozialformen sollte innerhalb eines Repositories einheitlich erfolgen.

Während der Bearbeitung kann dem Dateinamen ein Namenskürzel vorangestellt werden, beispielsweise `ch_01_008_0136_Prinzipien-Open-Science_I.md`.

---

## 4. Schritt-für-Schritt-Anleitung zur Entwicklung

### Schritt 1: Lernziel auswählen

Wählen Sie ein Lernziel aus der LZM-FDM aus.

Dokumentieren Sie:

- die vollständige Formulierung des Lernziels,
- die zugehörige LZM-ID,
- die Version der Lernzielmatrix,
- gegebenenfalls vorausgesetzte und weiterführende Lernziele.

Das Lernziel bildet die Grundlage für sämtliche zugehörigen Bricks.

### Schritt 2: Input-Brick erstellen

Öffnen Sie `template_I.md` und speichern Sie eine Kopie unter dem vorgesehenen Dateinamen.

Erarbeiten Sie die fachlichen Inhalte, die für das Lernziel relevant sind.

Achten Sie darauf, dass:

- die Inhalte unmittelbar zum Lernziel passen,
- Definitionen und zentrale Aussagen nachvollziehbar belegt sind,
- die Darstellung fachlich korrekt und verständlich ist,
- Beispiele einen Bezug zur Forschungspraxis herstellen,
- Quellen möglichst mit DOI oder dauerhaftem Link angegeben werden.

Der Input soll kompakt sein und sich auf die für das Lernziel wesentlichen Inhalte konzentrieren.

### Schritt 3: Aktivitäts-Bricks erstellen

Öffnen Sie `template_A.md` und erstellen Sie für die vorgesehenen Sozialformen jeweils eine eigene Datei.

Wählen Sie geeignete didaktische Methoden aus.

Beispiele:

| Sozialform | Mögliche Methoden |
|---|---|
| Plenum | Brainstorming, Lehrgespräch, gemeinsame Strukturierung |
| Gruppenarbeit | Sortieraufgabe, Begriffs-Puzzle, Fallanalyse |
| Partner:innenarbeit | Peer-Feedback, gegenseitige Erklärung, Zuordnungsübung |
| Einzelarbeit | Quiz, Reflexion, Begriffsdefinition |

Nicht jede Methode eignet sich gleichermaßen für jedes Lernziel. Die Auswahl sollte sich insbesondere am angestrebten Kompetenzniveau orientieren.

### Schritt 4: Didaktische Umsetzung beschreiben

Beschreiben Sie jede Methode so konkret, dass andere Lehrende sie ohne zusätzliche Rückfragen durchführen können.

Dazu gehören mindestens:

**Ziel der Methode:** Welche Teilkompetenz wird gefördert?

**Sozialform und Gruppengröße:** Für welche Zusammensetzung eignet sich die Methode?

**Zeitbedarf:** Wie lange dauert die Durchführung?

**Vorbereitung:** Was muss vor der Veranstaltung bereitgestellt werden?

**Ablauf:** Welche Arbeitsschritte erfolgen in welcher Reihenfolge?

**Materialien:** Welche Aufgaben, Texte, Beispielkarten oder digitalen Ressourcen werden benötigt?

**Ergebnissicherung:** Wie wird überprüft, ob das Lernziel erreicht wurde?

Bei Quizfragen oder Zuordnungsaufgaben sollten Musterlösungen bereitgestellt werden.

### Schritt 5: Input und Aktivitäten verknüpfen

Jeder Aktivitäts-Brick sollte auf den zugehörigen Input-Brick verweisen.

Dadurch können die fachlichen Grundlagen unabhängig von den didaktischen Aktivitäten gepflegt werden.

Auch der Input-Brick kann Links zu den zugehörigen Aktivitäten enthalten.

Verwenden Sie nach Möglichkeit relative Markdown-Links, damit die Verknüpfungen innerhalb eines GitHub-Repositories funktionieren.

### Schritt 6: Metadaten ergänzen

Jede Datei erhält die vorgesehenen Metadaten.

Dazu zählen insbesondere:

- `author`
- `email`
- `version`
- `language`
- `icon`
- `link`
- `licence`
- `comment`

Soweit weitere Metadatenfelder vorgesehen sind, beispielsweise `title`, `description`, `keywords`, `PublicationDate` oder `LearningResourceType`, sollten diese ebenfalls gepflegt werden.

Metadaten erleichtern die Auffindbarkeit, Zuordnung und Nachnutzung der Materialien.

### Schritt 7: Quellen und Lizenzierung prüfen

Verwendete Definitionen, Texte, Abbildungen, Videos und Methoden müssen mit geeigneten Quellenangaben versehen werden.

Bei externen Materialien sind die jeweiligen Nutzungsrechte zu beachten.

Für die bisher entwickelten Beispielmaterialien wird CC BY 4.0 verwendet. Ob diese Lizenz für einen neuen Brick angewendet werden kann, muss anhand der enthaltenen Materialien geprüft werden.

Informationen zur Lizenz: https://creativecommons.org/licenses/by/4.0/

### Schritt 8: Qualitätssicherung

Vor der Veröffentlichung sollten die Bricks fachlich, didaktisch und technisch geprüft werden.

Die Prüfung umfasst:

- Korrektheit der Inhalte
- Übereinstimmung mit dem Lernziel
- Verständlichkeit und sprachliche Qualität
- Vollständigkeit der Methodenbeschreibung
- Nachvollziehbarkeit der Aufgaben und Lösungen
- Funktion der Links
- Quellen und Lizenzangaben
- Lesbarkeit der Markdown-Dateien
- Nutzbarkeit in den vorgesehenen Lernumgebungen

---

## 5. Checkliste für Autor:innen

### Input-Brick

- [ ] Lernziel und LZM-ID korrekt angegeben
- [ ] Fachliche Inhalte auf das Lernziel abgestimmt
- [ ] Definitionen und Merkmale verständlich dargestellt
- [ ] Relevante Beispiele ergänzt
- [ ] Quellen und Links angegeben
- [ ] Metadaten vollständig
- [ ] Lizenzhinweise ergänzt

### Aktivitäts-Bricks

- [ ] Sozialform eindeutig angegeben
- [ ] Bezug zum Lernziel hergestellt
- [ ] Input-Brick verlinkt
- [ ] Methode verständlich beschrieben
- [ ] Ziel, Zeit und Gruppengröße angegeben
- [ ] Vorbereitung und Ablauf dokumentiert
- [ ] Materialien und Werkzeuge benannt
- [ ] Ergebnissicherung vorgesehen
- [ ] Aufgaben und Lösungen geprüft
- [ ] Quellen und Lizenzhinweise ergänzt

---

## 6. Hinweise zur Zusammenarbeit

Die Entwicklung kann kollaborativ über ein gemeinsames Repository erfolgen.

Empfohlen wird, dass Autor:innen:

1. eine Kopie des passenden Templates anlegen,
2. die Datei entsprechend der Namenskonvention benennen,
3. den Brick inhaltlich ausarbeiten,
4. Quellen und Metadaten ergänzen,
5. den Inhalt zur fachlichen und didaktischen Prüfung bereitstellen,
6. Rückmeldungen einarbeiten,
7. die freigegebene Fassung veröffentlichen.

Änderungen sollten nachvollziehbar dokumentiert werden. Eine Versionsverwaltung wie Git unterstützt die gemeinsame Entwicklung.

---

## 7. Weiterentwicklung und Nachnutzung

Die Templates sind als wiederverwendbare Grundlage gedacht.

Neue Lernziele können ergänzt werden, ohne bestehende Bricks verändern zu müssen.

Input-Bricks lassen sich mit unterschiedlichen Aktivitäts-Bricks kombinieren. Ebenso können vorhandene didaktische Methoden für andere Lernziele angepasst werden.

Bei jeder Anpassung sind die fachliche Passung, die Lizenzbedingungen und die Quellenangaben erneut zu prüfen.

---

## 8. Weiterführende Ressourcen

**Lernzielmatrix zum Forschungsdatenmanagement (LZM-FDM)**  
https://zenodo.org/records/15025246

**LiaScript – interaktive Lernmaterialien auf Markdown-Basis**  
https://liascript.github.io/

**Creative Commons BY 4.0**  
https://creativecommons.org/licenses/by/4.0/

---

## 9. Lizenzhinweise und Autor:innen

**Projekt:** OER.net FDM-Basiskurs

**Lizenz:** [bei Veröffentlichung ergänzen]

**Autor:innen dieser README:** [ergänzen]

**Kontakt:** [ergänzen]

**Version:** Entwurf 1.0

**Stand:** November 2026

---

*Diese README dient als Arbeitsgrundlage für die gemeinsame Entwicklung modularer, offen nachnutzbarer Lehr- und Lerninhalte zum Forschungsdatenmanagement.*
