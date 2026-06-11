# Wortmeister / Rote Lola 3

Interaktive Deutsch-Lernapp fuer die 3. Klasse auf Basis des Lehrmaterials
"Rote Lola 3". Die App uebersetzt die schriftlichen Uebungen in kurze,
smartphonefreundliche Trainingsrunden mit Fussball-/Turnieroptik.

Der Schwerpunkt liegt auf Wiedererkennung, klaren Wortbildern, grossen
Touchflaechen und stabilen Wiederholungen. Jede Aufgabe ist kurz, visuell
eindeutig und ohne freies Tippen spielbar.

## Ziel

Die App soll Grundschulkinder beim Wiederholen zentraler Rechtschreibstrategien
unterstuetzen:

- Woerter in Silben gliedern
- verwandte Woerter erkennen
- Woerter ableiten und verlaengern
- besondere Laute unterscheiden
- kurze und lange Vokale sichern
- Woerter im Woerterbuch vorbereiten
- Grossschreibung erkennen
- Fehler in Woertern und Saetzen finden

## Gestaltung

Die App ist mobile first aufgebaut und besonders fuer kleinere Smartphone-
Displays geeignet.

Gestaltungsprinzipien:

- dunkler Arena-Hintergrund
- tuerkise und helle Akzente im DFB-/Fussball-Look
- grosse Wortkarten
- grosse Antwortbuttons
- kurze Aufgabenstellungen
- visuelle Aufgabenmarker wie `ABC`, `GO`, `aa`, `i`, `..`, `!!`
- positive Rueckmeldung nach jeder Antwort
- keine Timer-Hektik
- keine Texteingabe durch das Kind

## Technik

Die App ist bewusst einfach und robust gehalten.

- reine HTML-Dateien
- CSS und JavaScript direkt in den jeweiligen Dateien
- kein Build-System
- keine externen Frameworks
- kein Server erforderlich
- lauffaehig per GitHub Pages
- JavaScript im ES5-Stil

Wichtig fuer neue Aenderungen:

- kein `let`
- kein `const`
- keine Arrow Functions
- keine modernen ES6+-Features
- keine HTML-IDs als automatische JavaScript-Variablen nutzen

## Struktur

```text
RoteLola/
├── index.html
└── klasse-3/
    ├── index.html
    ├── kapitel-1.html
    ├── kapitel-2.html
    ├── kapitel-3.html
    ├── kapitel-4.html
    ├── kapitel-5.html
    ├── kapitel-6.html
    ├── kapitel-7.html
    ├── kapitel-8.html
    ├── test-meilenstein-1.html
    ├── test-meilenstein-2.html
    ├── test-meilenstein-3.html
    └── test-meilenstein-4.html
```

## Kapitel

### Kapitel 1: Silbenmeister

Training zu Silbenpunkten, kurzen Namen und doppelten Mitlauten.

Beispiele:

- `Ida` bleibt ungetrennt
- `An..ton`
- `But..ter`
- `Tel..ler`

### Kapitel 2: Ableiten und Verlaengern

Training zu Wortfamilien, verwandten Woertern und sicheren Endlauten.

Beispiele:

- `Aeffchen` von `Affe`
- `Zaeune` von `Zaun`
- `runde` von `runder`
- `gelbe` von `gelber`

### Kapitel 3: Besondere Laute

Training zu `x`, `chs`, `v` und `f`.

Beispiele:

- `Hexe`
- `Dachs`
- `Experiment`
- `Vogel`
- `Fuchs`

### Kapitel 4: Kurze Vokale

Training zu `ck` und `tz` nach kurzem Vokal.

Beispiele:

- `Ecke`
- `witzig`
- `spritzt`
- `Versteck`
- `flitzt`

### Kapitel 5: Woerterbuch

Training zu Alphabet, Grundformen, Fremdwoertern, Fehlerwoertern und
zusammengesetzten Woertern.

Beispiele:

- Mehrzahl zur Einzahl zurueckfuehren
- Verbformen zur Grundform fuehren
- Fremdwort und Bedeutung verbinden
- Fehlerwoerter vergleichen

### Kapitel 6: Vokal-Zwillinge

Training zu doppelten Selbstlauten, Reimwoertern, langem `i` und Silben.

Beispiele:

- `Meer`
- `Boot`
- `Aal`
- `Kaffee`
- `Ki..no`
- `Me..di..zin`

### Kapitel 7: Grossschreibung

Training zu Nomen, Satzanfaengen, Zeitangaben, Namen und hoeflicher Anrede.

Beispiele:

- `die Bruecke`
- `am Dienstag`
- `im Maerz`
- `Wir danken Ihnen`
- `Moni und David`

### Kapitel 8: Fehler-Faenger

Training zum Erkennen und Korrigieren fehlerhafter Woerter.

Beispiele:

- `kikt` -> `kickt`
- `Fussbalverein` -> `Fussballverein`
- `Wannenrant` -> `Wannenrand`
- `Beuche` -> `Baeuche`

## Meilenstein-Tests

Jeder Meilenstein-Test prueft zwei Kapitel:

- Meilenstein 1: Kapitel 1 und 2
- Meilenstein 2: Kapitel 3 und 4
- Meilenstein 3: Kapitel 5 und 6
- Meilenstein 4: Kapitel 7 und 8

Die Tests enthalten jeweils 20 Fragen:

- 10 Fragen aus dem ersten Kapitel
- 10 Fragen aus dem zweiten Kapitel

Am Ende erscheint ein Zeugnis mit Trefferquote und Note. Fehler werden nach
Kapiteln getrennt gezaehlt. Es erscheinen nur die Wiederholungsbuttons fuer
Kapitel, in denen Fehler gemacht wurden.

## Notenschema

Die Note wird prozentbasiert vergeben:

- 96-100 Prozent: Note 1
- 80-95 Prozent: Note 2
- 60-79 Prozent: Note 3
- 45-59 Prozent: Note 4
- 16-44 Prozent: Note 5
- 0-15 Prozent: Note 6

Bei 20 Fragen entspricht eine Frage 5 Prozentpunkten.

## Lokal starten

Die App kann direkt im Browser geoeffnet werden. Fuer eine realistische lokale
Pruefung empfiehlt sich ein kleiner lokaler Server:

```powershell
python -m http.server 8765 --bind 127.0.0.1
```

Danach im Browser oeffnen:

```text
http://127.0.0.1:8765/
```

## GitHub Pages

Die App kann ohne Build-Schritt ueber GitHub Pages veroeffentlicht werden:

1. Repository auf GitHub oeffnen.
2. `Settings` auswaehlen.
3. `Pages` oeffnen.
4. Als Quelle den `main`-Branch auswaehlen.
5. Speichern.

Nach kurzer Zeit ist die App ueber die GitHub-Pages-Adresse erreichbar.

## Wartung

Wenn neue Inhalte ergaenzt werden, sollten sie direkt in der passenden
Kapiteldatei gepflegt werden. Neue Aufgaben werden als Datenobjekte im
jeweiligen JavaScript-Abschnitt angelegt.

Vor dem Hochladen sollte kurz geprueft werden:

- laedt die Datei im Browser?
- bleiben die Buttons auf Smartphonebreite gut lesbar?
- gibt es keine horizontalen Scrollbalken?
- bleibt JavaScript im ES5-Stil?

