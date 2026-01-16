---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.5
    </div>
  footerTemplate: |-
    <div style="font-size: 8px; width: 100%; display: flex; justify-content: space-between; padding: 0 20px; color: #78716c; font-family: 'Cinzel', serif;">
      <span>Nano Dungeon Engine</span>
      <span>Page <span class="pageNumber"></span> of <span class="totalPages"></span></span>
    </div>
  margin:
    top: "20mm"
    bottom: "20mm"
    left: "20mm"
    right: "20mm"
generated_at: "2026-01-16T08:33:24.495Z"
---


<style>
    body > h1:first-of-type, .markdown-body > h1:first-of-type { 
        text-align: center; 
        font-size: 2.5em; 
        border-bottom: 2px solid #b91c1c; 
        padding-bottom: 0.5em;
        margin-bottom: 2em;
    }
</style>

<style>
    h1 { color: #1c1917; }
    
    /* Dice & Tokens */
    .rpg-token {
        display: inline-block;
        padding: 0 0.3em;
        border-radius: 0.25em;
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;
        white-space: nowrap;
        font-size: 0.9em;
    }
    .token-d4 { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-d6 { background-color: #e2e8f0; color: #1e293b; border: 1px solid #94a3b8; }
    .token-d8 { background-color: #bfdbfe; color: #1e40af; border: 1px solid #60a5fa; }
    .token-d10 { background-color: #d8b4fe; color: #6b21a8; border: 1px solid #c084fc; }
    .token-d12 { background-color: #fbcfe8; color: #9d174d; border: 1px solid #f472b6; }
    .token-d20 { background-color: #bbf7d0; color: #166534; border: 1px solid #4ade80; }
    .token-tn { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-luck { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-power { background-color: #e9d5ff; color: #6b21a8; border: 1px solid #c084fc; }
    .token-heart { background-color: #fecaca; color: #991b1b; border: 1px solid #ef4444; }
    .token-stat { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-math { background-color: #1e293b; color: #38bdf8; border: 1px solid #0f172a; }
    
    /* Footer Styling */
    .pdf-footer {
        font-family: 'System-ui', sans-serif;
        font-size: 9px;
        color: #78716c;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
        border-top: 1px solid #e7e5e4;
        padding-top: 8px;
    }
    .footer-logo { height: 16px; vertical-align: middle; opacity: 0.6; margin-left: 10px; }
    
    /* Density Adjustments */
    h1, h2, h3, h4 { margin-top: 1em; margin-bottom: 0.5em; }
    p, ul, ol, blockquote { margin-bottom: 0.6em; }
    hr { margin: 1.5em 0; border: 0; border-top: 1px solid #e7e5e4; }
</style>
# Spielleiterhandbuch

Automatic translation placeholder for de

---



---

### 0) Spielregeln in 30 Sekunden

- **Fange mit der Fiktion an.** Beschreibe zuerst die Situation und die Aktionen der Spieler, dann erst den Test. 
- **Lege den Einsatz vor dem Wurf fest.** Sage, *was auf dem Spiel steht* und *was bei einem Misserfolg passieren wird*. 
- **Eine Entscheidung → ein Wurf → sinnvolles Ergebnis.** Teile eine Absicht nicht in drei Tests auf. 
- **Misserfolg treibt das Spiel voran.** „Resette“ die Szene nicht – ändere sie mit Komplikationen, Kosten oder Druck. 
- **Halte die Konsistenz.** Gleiche Bedingungen → ähnlicher Schwierigkeitsgrad, ähnliche Konsequenzen. 
- **Das Gitter ist optional.** Standardmäßig funktioniert das Spiel ohne Karte: „Nah / Weiter weg / Weit / Sehr weit entfernt“. 



---

### 1.1. Wann sollte man würfeln?

Ein Wurf macht nur dann Sinn, wenn gleichzeitig:
- das Ergebnis **nicht offensichtlich** ist,
- es einen **realen Einsatz** gibt (etwas wird sich ändern),
- beide Seiten akzeptieren, dass **die Mechanik das Recht hat zu entscheiden**.

**Nicht würfeln**, wenn:
- die Handlung routinemäßig und ohne Druck ist,
- ein Scheitern nichts Interessantes bringt,
- der Erfolg sicher ist und der Preis bereits bezahlt wurde (z. B. die Spieler haben Zeit, Werkzeuge und Sicherheit).

**Beispiel (ohne Wurf):** Ein Spezialist hat administrativen Zugang und ruhige Bedingungen – das Öffnen einer Standardtür in der Basis erfordert keinen Test.
**Beispiel (mit Wurf):** Dieselbe Tür, aber der Alarm ist aktiv, und eine Patrouille nähert sich in 30 Sekunden – das ist ein Test, weil der Einsatz Zeit und Entdeckung sind.

### 1.2. Entscheidungs-Checkliste (Tischverfahren)

1) Der Spieler sagt: **was er tut** und **was er erreichen möchte**. 
2) Du antwortest: **was im Weg steht** und **was auf dem Spiel steht**. 
3) Ihr wählt ein Attribut: **Kraft (K)** / **Geschicklichkeit (G)** / **Macht (<span class="rpg-token token-stat">M</span>)**. 
4) Du legst die **Schwierigkeit (<span class="rpg-token token-stat">S</span>)** oder die **Verteidigung** (im Kampf) fest. 
5) Du bestimmst den Situationsmodifikator: **Erhöhung/Reduzierung des Würfels** sowie eventuell **Hilfe**. 
6) Wurf → Ergebnis → Konsequenz → Szenenaktualisierung.

Kurz: **Beschreibung → Einsatz → Attribut → <span class="rpg-token token-stat">S</span>/Verteidigung → Wurf → Konsequenz**.

### 1.3. Schwierigkeit (T): Skala und praktische Regeln

Verwende eine einheitliche Skala im gesamten Spiel. Das baut das Vertrauen der Spieler in die Entscheidungen des Spielleiters auf.

- **T 3 – einfach:** günstige Bedingungen, kein Druck, minimaler Widerstand.
- **T 4 – Standard:** „normale Aufgabe“ in einem Abenteuer.
- **T 5 – schwierig:** Zeitdruck, Risiko, Gegner, begrenztes Zeitfenster.
- **T 6 – sehr schwierig:** deutlicher Vorteil des Gegners, hohes Risiko, komplexe Handlung unter Stress.
- **T 8 – heroisch:** überdurchschnittliche Leistung; erfordert in der Regel einen Vorteil, Plan oder Ressource.
- **T 12 – legendär:** „Wow“-Moment; selten ohne Vorbereitung und oft mit hohen Kosten.

**Praktische Regel:** Wenn du unsicher bist, welche Schwierigkeit festzulegen ist - beginne mit **T 4** und rechtfertige erst dann „nach oben“ oder „nach unten“. 

### 1.4. Modifikatoren ohne <span class="rpg-token token-stat">Z</span>ählen: Würfel erhöhen/senken

Anstelle von Boni und Strafen hinzuzufügen, änderst du in NDE die **Größe des Würfels** für einen Test.

- **Bessere Situation:** Erhöhe den Würfel um 1 Stufe  
  <span class="rpg-token token-<span class="rpg-token token-d4">d4</span>"><span class="rpg-token token-d4">k4</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">d8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">d12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">d20</span>"><span class="rpg-token token-d20">k20</span></span>
- **Schlechtere Situation:** Reduziere den Würfel um 1 Stufe (in die andere Richtung).

**Hilfe eines Verbündeten:** kostet seine Aktion und gibt **eine Erhöhung des Würfels um 1 Stufe** für den jeweiligen Test.

**Beispiel:** Ein Schloss in der Stille (T 4) vs. ein Schloss im Regen und unter Beschuss (T 5 + Senkung des Würfels, wegen zitternder Hände und mangelnder Sichtbarkeit). 
Das funktioniert normalerweise besser als „T 6 und +2 und -1“.

---

### 1.5. Testergebnisse: Erfolg, Fehlschlag und Spielfluss

- **1 auf dem Würfel:** Fehlschlag + Komplikation (die Komplikation tritt auf jeden Fall ein).
- **Ergebnis < T:** Fehlschlag (aber die Situation ändert sich).
- **Ergebnis ≥ T:** Erfolg.
- **Höchstwert auf dem Würfel:** außergewöhnlicher Erfolg (zusätzlicher Vorteil).

#### Wie gestaltet man einen Fehlschlag, ohne das Spiel zu blockieren?
Bevor der Spieler würfelt, legen Sie 1–2 Arten von Kosten fest:
- **Zeit** (jemand schafft es, etwas schließt sich),
- **Position** (schlechter positioniert, aufgedeckt),
- **Ressource** (Ausrüstung, Munition, Energie, Machtpunkt),
- **Aufmerksamkeit** (Alarm, Verdacht, Spur).

**Beispiel (fail-forward):**
Der Spieler möchte eine Tür aufbrechen. Fehlschlag bedeutet nicht „du öffnest sie nicht“.
Fehlschlag bedeutet: „du öffnest sie, aber machst Lärm – die Patrouille ist jetzt in der Nähe und das Alarmniveau steigt“.




---

### 2) Eine Prise Glück (PG): Wie man die Dramaturgie unterstützt, ohne das Spiel zu verderben

Jeder Held beginnt die Sitzung mit **2 PG**. Es ist ein Werkzeug für die Spieler, aber der Spielleiter ist für seine „Wirtschaft“ am Tisch verantwortlich.

### 2.1. Wofür geben die Spieler ihre Ł<span class="rpg-token token-stat">S</span> aus?

Gib 1 Ł<span class="rpg-token token-stat">S</span> aus, um:
- einen **erneuten Wurf** durchzuführen (den besseren behalten),
- den **Würfel um 1 Stufe** für einen Wurf zu erhöhen,
- einen Misserfolg in einen **Erfolg mit Kosten** umzuwandeln (der SL fügt einen Preis hinzu).

### 2.2. Wann einen zusätzlichen BZ gewähren?

Der Spielleiter kann **+1 BZ** gewähren für:
- bewusst eingegangenes Risiko, das die Szene antreibt,
- Akzeptanz der Konsequenzen ohne „Aushandeln“,
- kreative, konventionsgemäße Lösung,
- sehr gutes Spiel der Beziehung, Motivation oder des Einsatzes.

**Hygieneregel:** sparsam zuweisen (1–2 pro Sitzung pro Person bei einem extrem großzügigen Spiel). BZ sollte der „Funke“ sein, nicht der <span class="rpg-token token-math">st</span>ändige Treibstoff.



---

### 3) Konflikt und Kampf

NDE sollte schnell kämpfen. Wenn der Kampf 60 Minuten dauert, bedeutet das fast immer: zu viele Gegner „mit <span class="rpg-token token-heart">HP</span>“ oder zu viele kleine Würfelwürfe.

### 3.1. Standardmäßig ohne Karte: Bühnendistanzen

Verwende vier Distanzen:
- **Nah** – in Reichweite (Nahkampf),
- **Nicht weit** – ein paar Schritte entfernt,
- **Weit** – auf der anderen Seite der Bühne,
- **Sehr weit** – Scharfschützen-/Fahrzeugdistanz.

In einer Runde hat der Charakter: **Bewegung + 1 Aktion**.  
Die Bewegung ändert normalerweise die Distanz um **1 Stufe** (Nicht weit→Nah).

**Beispiel:** Ein Krieger ist Nicht weit. In der Runde: er läuft (Nah) heran und greift an.

### 3.2. Option: Gitter – wenn Präzision gefragt ist

Wenn ihr auf einem Gitter spielt:
- Bewegung in der Runde: **bis zu 5 Felder**,
- diagonale Bewegungen erlaubt,
- schwieriges Gelände kann „2 Felder pro Betreten“ kosten (optional).

Alle anderen Regeln bleiben identisch.

### 3.3. Gegnerverteidigung und Schaden

Im Kampf wird anstelle der Schwierigkeit die **Verteidigung** verwendet (eine Art „Schwierigkeit für den Kampf“).

**Verteidigung (Richtwerte):**
- **Schwach** 4
- **Typisch** 5
- **Elite** 6
- **Boss** 8 (legendärer Boss 12)

**Angriff:** Wurf auf **<span class="rpg-token token-math">St</span>ärke** (Nahkampf) oder **Geschicklichkeit** (Fernkampf) gegen die Verteidigung.

**Schaden (Tempo):**
- Ein Treffer verursacht **1 Herz**,
- ein außergewöhnlicher Erfolg verursacht **2 Herzen** oder sorgt für einen starken Effekt (Entwaffnung, Umwerfen, aus dem Rhythmus bringen, Ablenkung).

**Handlanger und Eliten (empfohlenes Modell):**
- **Handlanger:** 1 Treffer = aus dem Kampf raus (besiegt, flieht, kampfunfähig).
- **Elite:** hat **2 Herzen** (oder „2 Treffer“), hat oft einen taktischen Vorteil.
- **Boss:** hat **3 Herzen** + 1–2 „Boss-Bewegungen“ (siehe 3.6).

Dies ermöglicht schnelle Kämpfe ohne Punkte zählen.

### 3.4. Deckung, Vorteil und „übersichtliches Gelände“

Anstatt die Regeln zu multiplizieren, benutze eine einheitliche Sprache: **Würfel steigen / Würfel sinken**.

- Leichte Deckung, Rauch, schlechter Winkel: **senke den Würfel des Angreifers** um 1 Stufe.
- Gute Position, Überraschung, Höhenvorteil: **erhöhe den Würfel** um 1 Stufe.
- Volle Deckung: Angriff ist unmöglich, solange sich die Situation nicht ändert.

**Beispiel:** Ein Scharfschütze im Fenster ist „Weit entfernt“ und hat Höhenvorteil → der Angreifer bekommt eine Senkung des Würfels.
Die Gruppe wechselt die Szene: Rauchgranate, Flankieren, Umgehen – und der Vorteil verschwindet.

### 3.5. Reihenfolge im Kampf ohne Initiativzählung

Empfohlenes, schnelles Schema:
1) **Spieler handeln** (in beliebiger Reihenfolge am Tisch).
2) **Gegner handeln**.
3) Wiederholen.

Dies ermöglicht es den Spielern, kurze Kombinationen zu planen, ohne den Tisch mit der Initiative zu belasten.

### 3.6. Wie man einen Boss interessant gestaltet (und nicht als ‚Schwamm für Schaden‘)

Ein Boss im NDE sollte haben:
- **Verteidigung 8** (oder 12 in der 'Staffelfinale'-Version),
- **3 Herzen**,
- **1–2 einzigartige Bewegungen**, die die Szene verändern.

**Beispielhafte Bewegungen des Bosses (universell):**
- **Zurückdrängen:** jemand, der getroffen wird, zieht sich um 1 Distanz zurück (Nah→Weiter weg) und verliert die Position.
- **Schutzdurchbruch:** Der Boss zerstört einen Schutz oder zwingt einen dazu, aus der Deckung zu kommen.
- **Unterstützung rufen:** 2 Handlanger oder eine Elite schließen sich an (am besten einmal pro Kampf).
- **Gefahrenzone:** Der Bereich wird gefährlich (Feuer, Strom, Runen) – wer darin bleibt, riskiert einen Test.

**Regel:** Die Bewegung des Bosses soll das Spielfeld verändern und nicht nur ‚mehr Schaden verursachen‘.

### 3.7. Moral und Verhalten von Feinden (leichte Prozedur)

Wenn:
- der erste Handlanger fällt, oder
- die Elite ihr erstes Herz verliert, oder
- der Boss sein zweites Herz verliert,

wirf einen <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>">W6</span> und entscheide:
- **1–2:** sie ziehen sich zurück / suchen Deckung / verhandeln,
- **3–4:** sie halten die Stellung,
- **5–6:** sie greifen aggressiv an.

Modifiziere um **+1,** wenn sie im Vorteil sind, **-1,** wenn sie verängstigt oder abgeschnitten sind.



---

### 4) Kräfte (<span class="rpg-token token-stat">M</span>) auf der Seite des Spielleiters: wie man sie bewertet und wie man das Tempo nicht verlangsamt

In NDE umfasst „Kraft“ Magie, Psionik, Kybernetik, Hacking, Charisma „auf einem Filmniveau“ – abhängig von der Welt.

### 4.1. Machtskala: Schwierigkeit und Kosten von Machtpunkten

- **Trick:** <span class="rpg-token token-stat">S</span> 4, Kosten 0–1 MP (kleiner, kurzer Effekt).
- **Standard:** <span class="rpg-token token-stat">S</span> 5, Kosten 1 MP (einzelnes Ziel, kurzer Sprung, Schild).
- **Stark:** <span class="rpg-token token-stat">S</span> 6, Kosten 2 MP (Bereich, Kontrolle, Heilung).
- **Groß:** <span class="rpg-token token-stat">S</span> 8–12, Kosten 3 MP (szenenverändernder Effekt).

**Tipp:** Wenn der Effekt die „Regeln der Szene ändern“ soll (eine Brücke aus Eis, ein Blackout im Viertel) – dann ist das eine Große Macht.

### 4.2. Konsequenzen des Scheiterns der Macht

Ein Misserfolg sollte spezifisch und unmittelbar sein:
- Verlust von MP (immer),
- Überlastung (Abfall der Position, Entblößung),
- Spur (digital/astral),
- Nebeneffekt in der Umgebung (Lärm, Blitz, Geruch, Echo).

**Beispiel:** Live-Hack im Kampf. Misserfolg: MP geht verloren und das System protokolliert den Eindringling – der „Konter-ICE“-<span class="rpg-token token-stat">Z</span>ähler aktiviert sich.

### 4.3. Verteidigung gegen Macht

Wenn es die Fiktion rechtfertigt, erlaube einen "Gegen-Test":
- **Gewandtheit** (Ausweichen, Reflex) oder
- **Macht** (Widerstand, Gegenritual, Barriere).

Der Gegen-Test sollte die Würfe nicht vervielfachen. Verwende ihn dort, wo es die Szene interessanter macht (z.B. Lähmung, Gedankenkontrolle).



---

### 5.1. Erstellen Sie Szenen in 5 Schritten

1) **Ziel der Szene:** Was die Gruppe erreichen soll (konkret).  
2) **Hindernisse:** 2–3 verschiedene Arten (Menschen, Geräte, Umgebung).  
3) **Bedrohung:** Gegner, Gefahren, Fallen, Zeitdruck.  
4) **<span class="rpg-token token-stat">Z</span>ähler (optional):** 3–5 Felder; Misserfolge bewegen den <span class="rpg-token token-stat">Z</span>ähler; am Ende tritt eine große Auswirkung ein.  
5) **Belohnung und Konsequenzen:** Was ändert sich durch den Erfolg, was ändert sich durch das Scheitern.

Dies ist der minimale „Szenenmotor“ – er funktioniert in Fantasy, Sci-Fi und Krimi.

### 5.2. <span class="rpg-token token-stat">Z</span>ähler (clocks) – einfache Version

Ein <span class="rpg-token token-stat">Z</span>ähler hat 3–5 Felder. Er füllt sich, wenn:
- ein Test mit einem Fehlschlag endet,
- jemand Lärm macht,
- die Feinde Zeit haben zu reagieren.

Wenn der <span class="rpg-token token-stat">Z</span>ähler voll ist, tritt eine Auswirkung ein:
- Alarm,
- Verstärkung,
- Wegsperrung,
- Verlust einer Ressource,
- Eskalation des Konflikts.

**Beispiel:** „Alarm 0/4“. Fehlschlag beim Schleichen = +1. Besondere Erfolge = -1 (optional).  
Wenn es 4/4 erreicht – erscheint eine Patrouille und die Türen werden verriegelt.

---

### 5.3. Wie man die „Schwierigkeit der Szene“ bestimmt, ohne alles zu zählen

Für ein Team von 3–5 Helden:

- **Einfach:** 3–5 Gefolgsleute oder eine Elite ohne Geländevorteile.  
- **Standard:** 6–8 Gefolgsleute oder Elite + 2–4 Gefolgsleute oder Umweltgefahr.  
- **Schwierig:** Boss + 2–4 Gefolgsleute oder 2 Eliten + 3–5 Gefolgsleute oder <span class="rpg-token token-stat">Z</span>ähler 3.  
- **Heroisch:** Boss + Unterstützung + Geländedruck + <span class="rpg-token token-stat">Z</span>ähler 3–5.

**Am wichtigsten:** Gelände und Deckung sind oft bedeutender als die Anzahl der Feinde.



---

### 6.1. Schleichen und Infiltration: „Alarm“

1) Setze den <span class="rpg-token token-stat">Z</span>ähler **Alarm 0/3 bis 0/5**.  
2) Jeder Fehlschlag = +1 Alarm.  
3) Spieler können den Alarm durch Aktionen verringern (z. B. falsches Signal, Sabotage) – das sind normale Proben.  
4) Bei Maximum tritt die Konsequenz ein: Patrouille, Verriegelung, Lockdown.

**Beispiel:** Das Team geht durch den Korridor. Der Spezialist will die Kameras umgehen (<span class="rpg-token token-stat">M</span>, T 5). Fehlschlag = +1 Alarm.  
Bevor er würfelt, weiß er, was er riskiert – und das ist der Schlüssel.

### 6.2. Verfolgung: „Verfolgungsdistanz“

Bestimme die **Distanz** in Schritten, z.B. **3** (durchschnittlich).  
Jede „Verfolgungsrunde“:  
- Der Flüchtende macht einen Test (<span class="rpg-token token-stat">Z</span> oder <span class="rpg-token token-stat">M</span>, abhängig von der Methode),  
- Der Verfolger macht einen Test,  
- Erfolg des Flüchtenden erhöht die Distanz, Erfolg des Verfolgers verringert sie,  
- Wenn die Distanz auf **0** fällt – Einholung,  
- Wenn sie auf **5** steigt – Flucht.  

Füge Hindernisse (Kurve, Menschenmenge, Barrikade) als Beschreibung + Würfelmodifikator hinzu.  

### 6.3. Untersuchung: „Hinweise statt Testmauer”

Regel: **Ein Schlüsselhinweis darf sich nicht in einem einzigen Test verfangen**. 
Wenn die Untersuchungsszene weitergehen soll, ist der Schlüsselhinweis verfügbar:
- automatisch (wenn die Spieler etwas Sinnvolles tun),
- oder nach einem Test, aber ein Fehlschlag gibt ihn „mit Kosten“ (Zeit, falsche Fährte, Alarm).

**Beispiel:** Untersuchung des Körpers. Erfolg: Sie erhalten die Wahrheit. Fehlschlag: Sie erhalten die Wahrheit, aber die Wache kommt oder jemand bemerkt sie.

### 6.4. Gesellschaftlicher Konflikt: Einsatz, Druck, Konsequenz

Machen Sie aus einem Gespräch keinen "Würfelkampf". Legen Sie fest:
- was der NPC will,
- was die Spieler wollen,
- was auf dem Spiel steht,
- wie viele "<span class="rpg-token token-stat">Z</span>üge" bis zum Showdown (<span class="rpg-token token-stat">Z</span>ähler 3–5) sind.

Tests **<span class="rpg-token token-stat">M</span>** (Einfluss, Bluff, Autorität) oder **<span class="rpg-token token-stat">Z</span>** (Intention lesen) verändern die Gesprächsposition.  
Ein Misserfolg bringt Kosten (schlechter Eindruck, Verlust einer Ressource, Zeit, Feindseligkeit).



---

### 7.1. Komplikationen beim Scheitern (würfle <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>)

1. Zeitverlust / jemand hatte Zeit zu reagieren.  
2. Offenlegung der Position / Alarmanstieg.  
3. Leichter Schaden: -1 Herz oder Ressourcenverlust.  
4. Schlechte Position: Verdrängung, Sturz, Entblößung.  
5. Verlust oder Beschädigung der Ausrüstung.  
6. Eine neue Bedrohung erscheint in der Szene.

### 7.2. Vorteile bei außergewöhnlichem Erfolg (würfle <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>">w6</span>)

1. Schneller (du sparst Zeit oder Bewegung). 
2. Leiser (kein Anstieg des Alarms). 
3. Ohne Kosten (z.B. ohne Magiepunkte zu verwenden / ohne Geländekonsequenzen). 
4. Größerer Effekt (größere Reichweite, zusätzliches Ziel). 
5. Bessere Position für einen Verbündeten (jemand erhält einen Würfelbonus bei der nächsten Aktion). 
6. Zusätzlicher Hinweis oder erzählerischer Vorteil.

### 7.3. Schneller Gegner-Eintrag (Notizformat)

> **Name — Verteidigung, Herzen, Taktik, Trick/Vorteil**

- **Handlanger:** Verteidigung 4–5, 1 Treffer = verschwindet.  
- **Elite:** Verteidigung 6, 2 Herzen, ein Vorteil (Beweglichkeit/Konter/Deckung).  
- **Boss:** Verteidigung 8 (oder 12), 3 Herzen, 1–2 Boss-Bewegungen.

**Beispiel (universell):**  
> **Wächter — Verteidigung 5, 1 Treffer, hält den Korridor, Rauchgranate (einmal)**



---

### 8) Sicherheit und Tischvereinbarung (Minimum)

- Legt fest, was ihr nicht spielt (Tabuthemen) und was ihr überspringt.  
- Vereinbart ein einfaches Signal, um eine Szene zu unterbrechen (z.B. „Stopp“ oder „Pause“).  
- Konflikte am Tisch lö<span class="rpg-token token-math">st</span> ihr durch Gespräche außerhalb der Fiktion, nicht durch wütende Entscheidungen.

Das verbessert die Spielqualität mehr als jede Mechanik.



---

### 9) Modularität und Entwicklung durch die Gemeinschaft: wie man es im Zaum hält

Wenn Sie NDE als „Engine“ entwickeln, ist es am einfachsten, die Gemeinschaft durch Pakete weiterzuentwickeln:

- **Genre-Paket** (Fantasy/Cyberpunk/Horror): Mapping der Kräfte, Liste der Vorteile, Ausrüstung, Gegner, 1–2 Verfahren (z. B. Angst, Verfolgungsjagd).  
- **Gegner-Paket:** 10–20 Einträge Lakai/Elite/Boss + Taktiken.  
- **Abenteuer-Paket:** 1-seitige Szenen mit <span class="rpg-token token-stat">Z</span>ählern und Einsätzen.

**Anforderung an die Qualität des Beitrags:** Jede neue Regel sollte haben:
- den Satz „wozu das dient“ (welches Problem es lö<span class="rpg-token token-math">st</span>),
- eine kurze Regelbeschreibung,
- ein Beispiel von 3–5 Zeilen.

Auf diese Weise werden die Ergänzungen den Kern nicht sprengen und für Neulinge lesbar bleiben.

