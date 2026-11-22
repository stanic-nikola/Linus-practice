# Hausaufgabe 01: Web Engineering

**Zeit:** etwa 90 Minuten · **Hilfsmittel:** VS Code und Live Server · **Abgabe:** deine bearbeiteten Dateien aus diesem Ordner

Diese Hausaufgabe übt die Grundlagen aus der ersten Sitzung an einem neuen Beispiel. Bearbeite die vier Teile der Reihe nach. Schreibe Erklärungen in eigenen Worten; bei Unsicherheit darfst du Dokumentation nachschlagen und notierst das in der Reflexion.

## 1. Theorie (15–20 Minuten)

Öffne [theory.md](theory.md) und schreibe deine Antworten direkt unter die neun Fragen. Kurze, verständliche Antworten reichen; ein Beispiel ist oft hilfreicher als eine auswendig gelernte Definition.

## 2. Praxisprojekt: Anmeldung zum Campus-Lernabend (40–50 Minuten)

Erstelle in `index.html` und `styles.css` eine kleine Seite für einen fiktiven Campus-Lernabend. Die Dateien enthalten TODO-Kommentare als Startpunkte. Die Seite soll ohne JavaScript und ohne Serverprogramm funktionieren.

### HTML

1. Prüfe die vorhandene HTML5-Grundstruktur und ergänze die Inhalte in `header`, `main` und `footer`. Die Seite soll einen passenden Titel im Browser-Tab haben.
2. Im `header` stehen eine Hauptüberschrift, ein kurzer Einführungssatz und eine Navigation mit funktionierenden Sprunglinks zu `#programm` und `#anmeldung`.
3. Im Abschnitt `#programm` stehen eine zweite Überschrift, ein Absatz mit Ort und Beginn sowie eine ungeordnete Liste mit **mindestens drei** Programmpunkten.
4. Im Abschnitt `#anmeldung` stehen eine zweite Überschrift, ein kurzer Hinweis und ein Formular. Verwende `action="#anmeldung"` und `method="get"`. Das ist nur eine lokale Demo: Der Browser zeigt die eingegebenen Werte in der URL; es werden keine Daten gespeichert.
5. Das Formular enthält diese Felder mit jeweils passendem `label`, eindeutiger `id` und dem angegebenen `name`:

   | Beschriftung | `type` | `name` | Pflichtfeld? |
   | --- | --- | --- | --- |
   | Vorname | `text` | `vorname` | ja |
   | E-Mail-Adresse | `email` | `email` | ja |
   | Wunschtermin | `date` | `termin` | ja |
   | Erinnerung per E-Mail | `checkbox` | `erinnerung` | nein |

   Ergänze einen Button zum Absenden. Das `for` jedes Labels muss auf die `id` seines Feldes zeigen. Das Kontrollkästchen erhält `value="ja"`.
6. Im `footer` steht ein kurzer Hinweis, dass die Seite eine Übung ist. Nutze die vorhandene Klasse `karte` für beide Inhaltsabschnitte.

### CSS

Setze die Gestaltung ausschließlich in der externen Datei `styles.css` um:

1. Verwende mindestens je einen **Elementselektor**, **Klassenselektor** und **ID-Selektor**, außerdem einen **gruppierten Selektor** und einen **Nachfahrenselektor**.
2. Gestalte `body` mit einem hellen Hintergrund (`#f3f7fb`), dunkler Schrift (`#1d2a35`) und einem gut lesbaren Abstand der Zeilen. Entferne den äußeren Standardabstand des Browsers.
3. Der Kopfbereich hat einen dunklen Hintergrund (`#17324d`), weiße Schrift und Innenabstand. Die Navigationslinks sollen ebenfalls weiß und voneinander getrennt sein.
4. Der Hauptinhalt ist höchstens `720px` breit und mittig. Auf schmalen Fenstern bleibt links und rechts Innenabstand.
5. Beide Karten haben einen weißen Hintergrund, einen sichtbaren dünnen Rahmen sowie Innenabstand und Abstand zueinander. Der Anmeldeabschnitt bekommt zusätzlich einen farbigen linken Rand (`#0b7285`).
6. Die beiden Überschriftenebenen erhalten gemeinsam keinen oberen Außenabstand. Sorge für gut erkennbare Abstände an Beschriftungen und Formularfeldern. Der Absende-Button soll einen sichtbaren Hintergrund und Rahmen haben.

**Selbstkontrolle:** Öffne `index.html` mit Live Server. Prüfe die Sprunglinks, die Beschriftungen der Felder und die Darstellung bei schmalem Browserfenster. Beim Absenden einer ausgefüllten Demo-Anmeldung dürfen Werte in der URL erscheinen; eine Bestätigung oder Speicherung ist nicht vorgesehen.

## 3. Klausurähnliche CSS-Aufgabe (15–20 Minuten)

Öffne `exam-exercise.html` und lies die vorhandene Struktur. **Ändere das HTML nicht.** Schreibe nur Regeln in `exam-exercise.css`, sodass genau diese Anforderungen erfüllt sind:

1. Das Element mit `id="standorte"` erhält `background-color: #eef4ff`.
2. Nur `li`-Elemente **innerhalb** von `#standorte` erhalten `padding: 8px`. Der andere Listenbereich bleibt davon unberührt.
3. Nur das Element mit `id="hauptbibliothek"` erhält `border: 2px solid #274690`.
4. Alle Elemente mit `class="barrierefrei"` erhalten `font-weight: bold`, auch außerhalb von `#standorte`.
5. Nur Links **innerhalb** von `#standorte` erhalten `color: #14532d`.

Öffne auch diese HTML-Datei mit Live Server und kontrolliere beide Listen. Achte besonders auf den Unterschied zwischen einer Regel für das Element mit einer ID und einer Regel für seine Nachfahren.

## 4. Reflexion (5 Minuten)

Beantworte am Ende von `theory.md` kurz: Was war leicht? Was war schwierig? Welche Begriffe möchtest du noch einmal besprechen? Hast du allein gearbeitet oder externe Quellen verwendet? Falls ja, welche?

## Start mit Live Server

Öffne diesen Ordner in VS Code. Klicke in `index.html` mit der rechten Maustaste und wähle **Open with Live Server**. Für Teil 3 öffne danach `exam-exercise.html` auf dieselbe Weise. Es sind keine Pakete oder zusätzlichen Installationen nötig, sofern Live Server bereits eingerichtet ist.
