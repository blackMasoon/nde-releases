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
generated_at: "2026-01-16T08:50:46.470Z"
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
# Monsterhandbuch

Automatic translation placeholder for de

---



---

### Wozu ist dieses Buch

Dieses Buch ist ein **Werkzeugkasten** zum Erstellen von Gegnern und Bedrohungen im NDE:
- schnell (in 2–5 Minuten),
- ohne das Berechnen von Werten,
- konsistent mit den Regeln aus den **Basic Rules** und dem **Spielleiterhandbuch**.

**Die wichtigste Annahme von NDE:** *nur die Spieler würfeln.*
Gegner "greifen nicht durch Würfelwurf an" — sie greifen durch **Druck in der Fiktion** an: sie stellen Hindernisse, erzwingen Tests, erzeugen Bedrohungen und Konsequenzen.



---

### 0. Glossar (Begriffe in diesem Buch)

- **Verteidigung**: Der Schwellenwert, den ein Gegner im Kampf treffen/überwinden muss. Der Spieler würfelt und vergleicht das Ergebnis mit der Verteidigung.
- **Schwierigkeit (<span class="rpg-token token-stat">S</span>)**: Der Schwellenwert für einen Test gegen die Umwelt, ein Phänomen, eine spezielle Bewegung oder einen Gegnertrick.
- **Herzen**: Wie viele Schadenspunkte eine Kreatur in dieser Szene erträgt.
- **Handlanger / Elite / Boss**: Die drei Stufen der „Wichtigkeit“ eines Gegners in einer Szene.
- **Erleichterung / Erschwernis**: Änderung des Spielerwürfels um eine Stufe (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>** / nach unten).
- **Spezialbewegung**: Eine aktive Fähigkeit eines Gegners, die die Situation verändert (oft bedingt sie einen K/<span class="rpg-token token-stat">S</span>/A-Test des Spielers).
- **Eigenschaft (passiv)**: Eine konstante Eigenschaft des Gegners (Rüstung, Flug, Resistenz, Gefahrenzone), die in der Regel Erleichterung/Erschwernis bietet oder den Einsatz verändert.



---

### 1. Wie der Gegner in NDE funktioniert (kurz gefasst)

Im NDE ist der Gegner einfach, aber „lebendig“ dank seines Verhaltens.

1) **Der Spieler handelt → der Spieler würfelt.**  
   - Nahkampfangriff: <span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>) vs. **Verteidigung** des Ziels.  
   - Fernkampfangriff: Geschicklichkeit (<span class="rpg-token token-stat">Z</span>) vs. **Verteidigung** des Ziels.  
   - Kräfte: Macht (<span class="rpg-token token-stat">M</span>) vs. **Schwierigkeit (T)** oder vs. Verteidigung (bei Angriff/Betäubung).

2) **Wenn der Spieler verfehlt / den Test verliert**, geht die Szene weiter: Es entsteht ein Kosten- oder Komplikationsereignis.  
   Im Kampf kann eine Kostenbedeutung haben:  
   - Verlust der Position,  
   - Verlust der Zeit,  
   - Eintritt in eine gefährliche Zone,  
   - oder ein **verlorenes Herz**, falls es Sinn macht (z.B. Nahkampf, Kreuzfeuer, Wirkungsbereich).

3) **Der Gegner „handelt“ ohne zu würfeln:**  
   Der Spielleiter beschreibt, was der Feind tut, und wenn es den Helden real gefährdet, dann:  
   - erzwingt er einen Test (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) gegen **Schwierigkeit (T)**,  
   - oder stellt eine Bedingung („solange nicht...“, „wenn du eintrittst in...“, „wer in der Nähe steht...“),  
   - oder verändert die Würfel der Spieler (Erleichterung/Erschwerung).

4) **Der Kampf ist verständlich, wenn der Feind eine Ein-Satz-Taktik hat.**  
   Jeder Statblock sollte enthalten: „was dieser Feind in der ersten Runde tut“ und „was er tut, wenn er einen Schlag einsteckt“.



---

### 2. Statblock — Format und Felder

Ein minimaler Statblock enthält nur das, was in der Szene benötigt wird.

> **Name — Klasse, Verteidigung, Herzen, Rolle, Mobilität, Fähigkeiten, Bewegungen, Taktik**

### 2.1 Pflichtfelder

- **Klasse:** Handlanger | Elite | Boss  
- **Verteidigung:** Die Zahl, die durchbrochen werden muss, um den Feind zu treffen/umgehen.  
- **Herzen:** Wie viele Treffer es aushält (in NDE ist ein „Treffer“ standardmäßig = 1 Herz).  
- **Rolle:** Welchen Druck es im Kampf erzeugt (siehe Kapitel 4).  
- **Mobilität:** Wie es sich bewegt (beschreibend durch Zonen; Raster ist eine Option).  
- **Fähigkeiten (passiv):** 1–2 kurze Eigenschaften.  
- **Bewegungen (aktiv):** 1 Bewegung (Elite) oder 2-3 Bewegungen (Boss).  
- **Taktik:** 1-3 <span class="rpg-token token-stat">S</span>ätze, wie der SL den Feind konsequent führen kann.

### 2.2 Optionale Felder (gut zu haben, wenn sie passen)

- **Reichweite:** wenn der Feind ein Fernkämpfer ist (z.B. „Weit“, „Sehr weit“).
- **Zone:** wenn der Feind einen gefährlichen Bereich erzeugt (Rauch, Feuer, Kraftfeld).
- **Schwäche:** klarer „Hebel“ für die Spieler (Wasser, UV-Licht, Signalstörung).
- **Belohnung / Spur:** was nach dem Besiegen bleibt (Beute, Spur, Information).
- **Varianten:** 1–2 schnelle Austauschmöglichkeiten (z.B. „anstatt Flug hat er Sprung“; „anstatt Feuer hat er <span class="rpg-token token-stat">S</span>äure“).

### 2.3 Beispiel eines Statblocks (universell)

**Wächter — Lakai, Verteidigung 5, Herzen 1, Grobian, Mobilität: Nahe→Eng, Fähigkeiten: Schild, Bewegungen: Ansturm, Taktik: blockiert den Durchgang und drängt aus Deckungen heraus.**

- **Schild (passiv):** solange er **Eng** an einer Deckung oder einem Schildträger steht, hat der Angreifer einen **Malus** (Würfel um 1 Stufe senken).
- **Ansturm (Bewegung):** wenn der Wächter im Nahkampf trifft (oder wenn der Spieler einen Nahkampfangriff gegen ihn verfehlt), kann der Spielleiter den Helden um 1 Zone (Eng→Nahe) oder um 1–2 Felder im Gittermodus verschieben.
- **Taktik:** greift das schwächste Ziel im Nahkampf an, verteidigt den Gang, flieht nicht.



---

### 3. Gegnerklassen: Handlanger, Elite, Boss

In NDE besteht die 'Schwierigkeit' eines Gegners aus zwei Dingen: - **wie schwer er zu treffen ist** (Verteidigung), - **wie viel er aushält** (Herzen), - und **welchen Druck er ausübt** (Rolle + Bewegungen).

### 3.1 Lakai (Handlanger)

- **Verteidigung:** normalerweise **5** (leichter: 4, schwieriger: 6).
- **Herzen:** **1** (fällt nach einem Treffer aus).
- **Bewegungen:** normalerweise 0–1 (einfach und durchschaubar).
- **Zweck:** sorgt für Tempo, Hintergrund und das Gefühl eines „Kampfes gegen eine Gruppe“.
- **Wie zu führen:** tritt in Gruppen von 3–8 auf, stirbt schnell, macht aber Lärm und beansprucht Raum.

> Gute Regel: Ein Lakai hat vor allem eine *Position* (Deckung, zahlenmäßiger Vorteil, hohe Lage) und keine „komplexe Mechanik“. 

### 3.2 Die Elite

- **Verteidigung:** normalerweise **6** (leichtere Elite: 5, „harte Elite“: 8).  
- **Herzen:** **2**.  
- **<span class="rpg-token token-stat">Z</span>üge:** 1 charakteristischer Zug + 1 passive Eigenschaft.  
- **Zweck:** ist ein „Mini-Boss“ in der Szene, zwingt zur Anpassung.

> Die Elite sollte *eine Sache deutlich* tun: „bricht Schutzschilde“, „stellt Zonen auf“, „springt an Wänden hoch“, „heilt Handlanger“.

### 3.3 Boss

- **Verteidigung:** normalerweise **8** (legendär: 12).
- **Herzen:** **3** (final: 5).
- **<span class="rpg-token token-stat">Z</span>üge:** 2–3 <span class="rpg-token token-stat">Z</span>üge + 1–2 passive Eigenschaften.
- **Wofür es da ist:** Es ist eine eigene Szene — beeinflusst das Gelände und das Tempo.

**Ein Boss ohne Tricks ist langweilig.** Damit ein Boss „spielbar“ ist, gib ihm mindestens eines der folgenden:
- einen Zug, der einen Test für viele Helden erzwingt,
- eine Zone (Gelände, das man beachten muss),
- oder eine „Phasen“-Mechanik (nach dem Verlust von 1 Herz ändert sich das Verhalten).

### 3.4 „Legendär” (optionale Stufe)

Falls du einen Kampagnengegner benötigst:
- **Verteidigung 12**, **Herzen 5**, 3–4 Bewegungen, Zonen und Phasen.
Dies ist ein „Endboss für den Akt“ — verwende ihn nicht zufällig.



---

### 4. Rollen der Gegner (deutlicher Druck)

Die Rollen sind dafür da, dass der Spielleiter sofort weiß, „wie man das spielt“.
Die Rolle ist keine Statistik — es ist ein **Stil der Bedrohung**.

- **Brute (Nahkampf):** tritt Nah heran, drückt, wirft um, durchbricht die Front.
  *Frage an die Spieler:* „Wer steht vorne und was riskiert er?“

- **Skirmisher (Mobil):** tritt ein, tut sein Werk und zieht sich zurück; bestraft die Einsamkeit.
  *Frage:* „Wer ist von der Gruppe getrennt?“

- **Artillery (Fernkampf):** schießt aus der Deckung; erzwingt Bewegung und Positionswechsel.
  *Frage:* „Wo ist es sicher, und wo ist die Schusslinie?“

- **Controller (Kontrolle):** Zonen, Rauch, klebriges Gelände, Fallen, Druck auf Ziele.
  *Frage:* „Wie umgeht man die Zone, anstatt in ihr zu kämpfen?“

- **Support (Unterstützung):** <span class="rpg-token token-math">st</span>ärkt, heilt, bewegt, bietet Deckung.
  *Frage:* „Wen schaltet man zuerst aus, um den Kampf zu vereinfachen?“



---

### 5. Erleichterungen/Erschwernisse bei Monstern — Leitregel

In NDE **komplizieren wir die Zahlen nicht**.
Statt: „+2 auf Treffer, -1 auf Schaden, Bonus auf AC“ — machen wir:

- **Erleichterung:** Steigere den Würfel des Spielers um 1 Stufe,
- **Erschwernis:** Verringere den Würfel des Spielers um 1 Stufe,
- **Änderung des Einsatzes:** Erfolg ist möglich, erfordert aber einen anderen Ansatz (z.B. zuerst die Deckung entfernen).

### 5.1 Wann ändert man die Verteidigung und wann den Würfel

- **Ändere meistens den Würfel des Spielers** (Erleichterung/Erschwerung).
- **Ändere die Verteidigung selten**, hauptsächlich wenn:
  - der Feind über „Rüstung / Unsichtbarkeit / ein Kraftfeld“ verfügt, die es *tatsächlich* schwerer machen, ihn zu treffen,
  - oder wenn es sich um eine Mechanik der Bossphase handelt.

### 5.2 Beispiele für 'reine' Erschwernisse

- „Der Feind hat eine teilweise Deckung“ → der Angreifer hat ein **Erschwernis**. 
- „Der Feind ist betäubt / gefesselt“ → der Angreifer hat ein **Vorteil**. 
- „Der Feind ist schnell und springt an den Wänden hoch“ → der Angreifer hat ein **Erschwernis**, bis er ihn blockiert.



---

### 6. Passive Fähigkeiten (Eigenschaften) — Katalog zum Zusammenfügen

Unten findest du Eigenschaften, die du an ein Statblock anfügen kannst. Wähle **1–2** (Boss: 2–3). Beschreibe sie immer im Kontext der Spielwelt.

### 6.1 Schutz und Härte

- **Leichte Rüstung:** Der erste Treffer in dieser Szene verursacht 1 Herz weniger (also 0) *oder* erfordert eine „Präzisierung“ (Erfolg verursacht erst dann ein Herz, wenn der Angriff die Rüstung umgeht).  
  *Einfachste Version:* „Der erste Treffer verursacht kein Herz.“

- **Schwere Rüstung:** Solange die Rüstung nicht umgangen wird (flankieren, Explosion, Haken, Magie), haben Angriffe **Erschwernis**.  
  *Hinweis:* Gib den Spielern einen klaren Weg, die Rüstung zu umgehen.

- **Hart:** Nach dem Verlust von 1 Herz ändert der Feind seine Position nicht (er kann nicht leicht herausgedrängt/umgestoßen werden).  
  Gut für Kolosse und Bosse.

### 6.2 Beweglichkeit

- **Schnell:** Einmal pro Runde kann eine zusätzliche Zone in der Distanz verändert werden (z. B. Weit→Nah). 
  Im Raster: +1–2 Felder.

- **Springer / Kletterer:** Behandelt vertikale Hindernisse als normal. 
  Bietet sinnvolle „Abkürzungen“ in den Rücken.

- **Fliegen:** Ignoriert Geländehindernisse, erfordert jedoch Deckung „von oben“ oder zwingt zu Reaktionstests (z. B. <span class="rpg-token token-stat">Z</span>, um einem Luftangriff zu entgehen).

### 6.3 Wahrnehmung und Schleichen

- **Späher:** Der erste Versuch, ihn aus dem Hinterhalt anzugehen, hat einen **Erschwerungsgrad**.
- **Wachen:** Wenn jemand in der Szene eine laute Aktion ausführt, wechselt der Feind sofort in eine bessere Position (geht in Deckung / ruft Unterstützung).

### 6.4 Widerstände und Schwächen (einfach)

- **Widerstand [Typ]:** Das erste Mal in einer Szene, wenn der Gegner einen bestimmten Effekt (Feuer, Eis, Psyche, Elektrizität) erhalten würde, ist der Effekt **schwächer** (kleinerer Bereich / kürzer / ohne Verlust von Herz).  
- **Schwäche [Typ]:** Gegen diesen Typ von Angriffen hat der Spieler einen **Vorteil**.

> Grundsatz der Transparenz: Widerstände und Schwächen sind nur sinnvoll, wenn die Spieler sie entdecken und nutzen können.

### 6.5 „Schwarm” und Druck der Anzahl

- **Schwarm:** Wenn sich mindestens zwei solcher Kreaturen in der Nähe eines Helden befinden, hat der Held **Erschwerung** bei Bewegungs-/Fluchttests, bis er die Zone wechselt.



---

### 7. Aktive Aktionen — wie man schreibt und wie man führt

Eine aktive Aktion sollte drei Fragen beantworten: 1) **Was macht sie in der Fiktion?** (Beschreibung) 2) **Wen betrifft sie und wann?** (Auslöser) 3) **Wie wird sie mechanisch entschieden?** (Test / Effekt / Kosten)

### 7.1 Einfaches Bewegungsformat

- **Bewegungsname:** ein Satz der Beschreibung.
- **Auslöser:** wann es passiert (z.B. „wenn der Held in der Nähe ist“, „wenn jemand aus der Deckung schießt“).
- **Test:** welche Eigenschaft und welcher Schwierigkeitsgrad.
- **Folge eines Fehlschlags:** was du verlierst, was sich ändert.
- **Folge eines Erfolgs:** normalerweise vermeidest du die Folge oder erhältst einen Vorteil.

### 7.2 Wie wird die Schwierigkeit einer feindlichen Bewegung festgelegt (ohne Tabellen)

Wenn die Bewegung „angreifend“ ist und sich auf ein einzelnes Ziel bezieht:
- setze **T der Bewegung = Verteidigung des Feindes** (das ist konsistent und leicht zu merken).

Wenn die Bewegung flächendeckend oder „groß“ ist:
- setze T 1 Schwelle höher als der Standardschwellenwert der Szene (normalerweise **T 6** oder **T 8**).

### 7.3 Beispielzüge (Module)

**Ansturm (Brute)**  
- **Beschreibung:** Der Feind geht in den Nahkampf und drängt zurück.  
- **Auslöser:** Wenn der Feind in der Nähe des Helden ist.  
- **Test:** Der Held macht einen Test auf **<span class="rpg-token token-stat">S</span> oder <span class="rpg-token token-stat">Z</span>** gegen **T = Verteidigung des Feindes**.  
- **Misserfolg:** Der Held verliert 1 Herz *oder* wird um eine Zone zurückgeschoben (die Spielleitung wählt, was sinnvoll ist).  
- **Erfolg:** Du vermeidest Schaden und hältst deine Position.

**Salve (Artillery)**  
- **Beschreibung:** Eine Serie von Schüssen/Splittern in ein Gebiet.  
- **Auslöser:** Wenn mindestens 2 Helden in derselben Zone und nicht in Deckung sind.  
- **Test:** Jeder Zieltest **<span class="rpg-token token-stat">Z</span>** gegen **T 6** (oder T = Verteidigung des Feindes, wenn der Feind Elite ist).  
- **Misserfolg:** −1 Herz und „du musst dich bewegen“ (Nah→Fern).  
- **Erfolg:** Du versteckst dich/nimmst keinen Schaden.

**Anker (Controller)**  
- **Beschreibung:** Klebriger Boden, Kraftfeld, Spinnennetz, Eis.  
- **Auslöser:** Der Feind hat einen Moment, um die Zone einzurichten.  
- **Test:** Wenn du in die Zone eintrittst, teste **<span class="rpg-token token-stat">Z</span> oder <span class="rpg-token token-stat">M</span>** gegen **T 5–6**.  
- **Misserfolg:** Du verlierst die Bewegung in dieser Runde und bist „in schlechter Position“ (Erschwerung bei Angriffen).  
- **Erfolg:** Du gehst hindurch oder neutralisierst die Zone.

**<span class="rpg-token token-math">St</span>ärkung (Support)**  
- **Beschreibung:** Der Feind deckt einen Verbündeten/ heilt/ gibt einen Vorteil.  
- **Auslöser:** Einmal pro Runde, wenn ein Verbündeter bedroht wird.  
- **Effekt:** Der gewählte Verbündete erhält einen „Schild“ — Angreifende haben **Erschwerung** bis zum Ende der Runde, oder der Verbündete erholt 1 Herz (Boss/Elite).  
- **Spielerkonter:** Deaktiviere den Supporter oder zwinge ihn, zu wählen (wen er rettet).  




---

### 8.1 Standardmäßig: Distanzzonen

Im erzählerischen Kampf benutze: **Nah / Etwas entfernt / Weit entfernt / Sehr weit entfernt**.

Im Statblock notiere Mobilität als:
- „**Mobilität:** ändert die Zone um 1 (Standard)“
- oder „**Mobilität:** Schnell (ändert die Zone um 2)“
- oder „**Mobilität:** Fliegen (ignoriert Hindernisse, erfordert aber Tests bei Angriffen aus der Luft)“. 

### 8.2 Option: Raster (falls der Tisch Taktik mag)

Wenn ihr auf einer Karte spielt:
- Standardbewegung = **5 Felder**,
- Schnell = **6–7**,
- Sprung = 3 Felder „in die Höhe“ oder über Hindernisse.

**Alle beschreibenden Fähigkeiten funktionieren genauso** – das Raster „gibt nur ein Maßband her“.



---

### 9. Gegner in 2 Minuten erstellen (Vorgehensweise)

1) **Wähle eine Klasse**: Handlanger / Elite / Boss. 
2) **Setze Verteidigung**: 5 / 6 / 8 (legendär: 12). 
3) **Setze Herzen**: 1 / 2 / 3 (final: 5). 
4) **Wähle eine Rolle**: Prügler / Scharmützler / Artillerie / Kontrolle / Unterstützung. 
5) **Füge 1–2 passive Eigenschaften hinzu** (Boss: 2–3). 
6) **Füge Bewegungen hinzu**: Elite 1, Boss 2–3. 
7) **Schreibe eine Strategie in 2 <span class="rpg-token token-stat">S</span>ätzen** (erste Runde + Reaktion auf Gefahr). 
8) (Optional) Füge **Schwäche** und **Belohnung** hinzu.

> Praktischer Test: Wenn du den Gegner ohne Blick auf die Tabelle führen kannst – ist der Statblock gut.



---

### 10. Fertige Vorlagen (für Reskin in jeder Welt)

Die folgenden Einträge sind absichtlich 'farblos'. Du änderst den Namen und die Beschreibung – die Mechanik bleibt.

### 10.1 Handlanger

- **Wächter — Handlanger, Verteidigung 5, Herzen 1, Grobian, Mobilität: Standard, Fähigkeiten: Schild, Bewegungen: Ansturm, Taktik: blockiert und <span class="rpg-token token-math">st</span>ößt zurück.**
- **Späher — Handlanger, Verteidigung 5, Herzen 1, Scharmützler, Mobilität: Schnell, Fähigkeiten: Kundschafter, Bewegungen: Flucht, Taktik: nähert sich, markiert Ziele und verschwindet.**
- **Schütze — Handlanger, Verteidigung 5, Herzen 1, Artillerie, Mobilität: Standard, Fähigkeiten: Deckung, Bewegungen: Beschuss, Taktik: hält auf Distanz und zwingt zum Rennen.**
- **Kontrolleur — Handlanger, Verteidigung 5, Herzen 1, Kontrolleur, Mobilität: Standard, Fähigkeiten: Zone, Bewegungen: Anker, Taktik: spaltet das Team.**
- **Unterstützer — Handlanger, Verteidigung 5, Herzen 1, Unterstützung, Mobilität: Standard, Fähigkeiten: Sanitäter, Bewegungen: Verstärkung, Taktik: schützt die Elite.**

**Schnelle Bewegungen für Handlanger:**
- **Flucht:** zieht sich um 1 Zone zurück, wenn er getroffen wird (aber noch nicht 'ausgeschaltet' ist, z.B. in einer Rüstungsszene).
- **Beschuss:** wenn jemand im Offenen steht, erschwert es die nächste Aktion für ihn ('Kugeln, Splitter, Angst').
- **Zone:** legt einmal pro Szene eine kleine Hinderniszone an (Rauch, Öl, Matsch).

### 10.2 Elite

- **Kämpfer — Elite, Verteidigung 6, Herzen 2, Brute, Mobilität: Standard, Fähigkeiten: Leichte Rüstung, Bewegungen: Drang, Taktik: kommt nahe heran und hält die Linie.**
- **Attentäter — Elite, Verteidigung 6, Herzen 2, Skirmisher, Mobilität: Schnell + Springer, Fähigkeiten: Späher, Bewegungen: Flankenschlag, Taktik: schlägt von hinten zu und zieht sich zurück.**
- **Scharfschütze — Elite, Verteidigung 6, Herzen 2, Artillery, Mobilität: Fern, Fähigkeiten: Deckung, Bewegungen: Zielschuss, Taktik: erzwingt Bewegung und bestraft mangelnde Deckung.**
- **Gelände-Manipulator — Elite, Verteidigung 6, Herzen 2, Controller, Mobilität: Standard, Fähigkeiten: Zone (2×), Bewegungen: Anker, Taktik: schneidet Fluchtwege ab.**
- **Kommandant — Elite, Verteidigung 6, Herzen 2, Support, Mobilität: Standard, Fähigkeiten: Sensoren, Bewegungen: Verstärkung, Taktik: verstärkt Verbündete und positioniert sie in der Deckung.**

### 10.3 Bosse

- **Anführer — Boss, Verteidigung 8, Herzen 3, Unterstützung, Mobilität: Standard, Fähigkeiten: Wachsamkeit + Schild, Bewegungen: Verstärkung + Beschwörung + Barriere, Taktik: hält Unterstützung und kontrolliert das Tempo.**
- **Koloss — Boss, Verteidigung 8, Herzen 3, Schläger, Mobilität: Standard, Fähigkeiten: <span class="rpg-token token-stat">Z</span>äh + Schwergepanzer, Bewegungen: Erschütterung + Ansturm, Taktik: zerschlägt die Aufstellung und erzwingt Tests.**
- **Jäger — Boss, Verteidigung 8, Herzen 3, Scharmützler, Mobilität: Schnell + Springer, Fähigkeiten: Späher, Bewegungen: Hinterhalt + Schnitt + Flucht, Taktik: isoliert und eliminiert.**
- **Zonenarchitekt — Boss, Verteidigung 8, Herzen 3, Kontrolleur, Mobilität: Standard, Fähigkeiten: Zone (2×) + Resistenz [Typ], Bewegungen: Anker + Salve + Verschiebung, Taktik: teilt die Gruppe und zwingt zu Entscheidungen.**



---

### 11. Umweltgefahren (Gefahren)

Gefahr ist ein „Gegner ohne Willen“ oder ein Szenemechanismus: ein Geschützturm, Feuer, Lawine, Alarm.  **Format: Name — Schwierigkeitsgrad (T), Wann es wirkt, Wirkung, Wie man es deaktiviert / umgehen kann**

### 11.1 Beispiele für Gefahren (universal)

**Geschützturm / Verteidigungsdrohne — T 6**  
- **Wann es funktioniert:** am Ende der Runde, wenn sich jemand in der Linie befindet.  
- **Folge:** Test **<span class="rpg-token token-stat">Z</span> gegen T 6**; Misserfolg: −1 Herz und du musst in Deckung gehen.  
- **Deaktivierung:** Test **<span class="rpg-token token-stat">M</span> oder <span class="rpg-token token-stat">Z</span> gegen T 6** am Panel / <span class="rpg-token token-math">St</span>ören / Stromunterbrechung.

**Falle / Mine / Stolperfalle — T 5**  
- **Wann es funktioniert:** wenn du die Zone betrittst.  
- **Folge:** Test **<span class="rpg-token token-stat">Z</span> gegen T 5**; Misserfolg: −1 Herz oder Immobilisierung (du verlierst die Bewegungsfähigkeit).  
- **Deaktivierung:** Werkzeuge + Test **<span class="rpg-token token-stat">Z</span> gegen T 4–5**.

**Gas / Rauch / Verseuchung — T 5**  
- **Wann es funktioniert:** am Anfang der Runde, wenn du in der Zone bist.  
- **Folge:** Test **<span class="rpg-token token-stat">S</span> oder <span class="rpg-token token-stat">M</span> gegen T 5**; Misserfolg: −1 Herz oder Erschwernis für Tests, um das Gebiet zu verlassen.  
- **Deaktivierung:** Belüftung, Masken, Abdichtung.

**Alarm / Timer — T (szeneabhängig)**  
- **Wann es funktioniert:** wenn eine Komplikation eintritt oder jemand Lärm macht.  
- **Folge:** Zeitdruck entsteht (nächste Welle, Türen schließen, Verstärkungen).  
- **Deaktivierung:** Test **<span class="rpg-token token-stat">M</span>** (Hacken/Ritual) oder „physisch“ Test **<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>**.



---

### 12. Kampf Szenengenerator (schnell, leserlich)

Wählen Sie jeweils 1 aus jeder Zeile (oder werfen Sie <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>):

1) **Ziel der Szene:** Durchgang / Wiedererlangung / Deaktivierung / Eskortierung / Diebstahl / Verteidigung  
2) **Gebiet:** offen / Engpässe / mehrstöckig / viel Deckung / Kanten / Nebel-Rauch  
3) **Gegner:** 6× Handlanger / 4× Handlanger + Elite / 2× Elite / Boss / Boss + 2× Handlanger / Elite + Risiko  
4) **Vorteil des Feindes:** Deckung / Höhe / Mobilität / Zeitdruck / Hinterhalt / Fernunterstützung  
5) **Vorteil der Spieler:** Überraschung / Werkzeuge / Abkürzung / neutraler Verbündeter / Gebiet bietet Deckung / Information (sie kennen den Feind)



---

### 13. Balance in der Praxis (ohne Mathematik)

Im NDE wird das Gleichgewicht durch *Tempo* und *Druck* erreicht, nicht durch „CR“.

### 13.1 Schnellregeln zur Festlegung des Schwierigkeitsgrads einer Szene

- **Einfache Szene:** 4–6 Handlanger oder 1 Elite.  
- **Standard-Szene:** 4 Handlanger + 1 Elite, oder 2 Elites.  
- **Schwierige Szene:** Boss + 2–4 Handlanger, oder Boss + Gefahr.  
- **Finale:** Boss (Herz 5) + Elite + Zeitdruck.

### 13.2 Wenn der Kampf zu kurz dauert

- Schicke eine **Welle von Handlangern** (2–3 pro Runde für 2 Runden). 
- Erhöhe den Druck des Geländes: Rauchzone, Alarm, fehlende Deckung. 
- Ändere die Taktik: Der Feind hört auf, „fair“ zu kämpfen (er zieht sich zurück, nimmt Geiseln, blockiert den Ausgang).

### 13.3 Wenn sich der Kampf hinzieht

- Gib den Spielern einen „Hebel“: aufgedeckter Tank, Panel, Ritual, Schwäche.  
- Erlaube **Vorteile bei außergewöhnlichem Erfolg**: Durchbrechen der Deckung, Entwaffnung, <span class="rpg-token token-math">St</span>örung der Unterstützung.  
- Reduziere die Herzen des Bosses von 5 auf 3, wenn es sich nicht um das Finale handelt.



---

### 14. Reskin: wie man einen Feind für jedes Setting umgestaltet

Du hast den Statblock 'Späher'. Jetzt änderst du nur die Beschreibung:

- **Fantasy:** Goblin-Bogenschütze-Späher (Späher + Beschuss).  
- **Sci-fi:** Aufklärungsdrohne (Späher + Sensoren).  
- **Cyberpunk:** Gang-Scout auf einem Skateboard (Schnell + Flucht).  
- **Slawisch:** Dämon, der den Spuren folgt (Empfindlichkeit: Eisen; Resistenz: Angst).

Die Mechanik bleibt dieselbe. Dies ermöglicht es der Community, hunderte von Einträgen hinzuzufügen, ohne die Konsistenz des Kerns zu zerstören.

