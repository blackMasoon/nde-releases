---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.4
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
generated_at: "2026-01-15T07:57:22.444Z"
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
# Regeln auf einen Blick

Automatic translation placeholder for de

---



---

### 1) Held in 1 Minute


* **Konzept:** wer bist du und in welchem Genre spielst du (1 Satz).
* **Rolle (wähle eine):**

  * **Sturm** – Druck, Kampf, Überwinden von Hindernissen
  * **Spezialist** – Schleichen, Präzision, Technik, Beobachtung
  * **Adept** – Kräfte, Wissen, Einfluss, Improvisation
* **Eigenschaften (3):**

  * **<span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>)** – körperliche <span class="rpg-token token-math">St</span>ärke, Ausdauer, Nahkampf
  * **Geschicklichkeit (G)** – Reflexe, Schleichen, Schießen, Steuern
  * **Macht (<span class="rpg-token token-stat">M</span>)** – Magie/Psionik/Technologie/Bluff/Intuition (je nach Welt)
* **Würfel für Eigenschaften:** ein Würfel **<span class="rpg-token token-d12">k12</span>**, ein **<span class="rpg-token token-d8">k8</span>**, ein **<span class="rpg-token token-d6">k6</span>** (wähle entsprechend der Rolle).
* **Herzen:** 5. **Machtpunkte:** 3 (verwendest du für Kräfte und „besondere Aktionen“).
Unten hast du einen fertigen Abschnitt zum Einfügen (Variante A), im Stil der kurzen Regeln „1-Seite“.

**Wurf des Glücks (wie es funktioniert):** gib **1 WdG** aus, um eines auszuwählen:

* **Wiederwurf** deines Tests (du behältst das bessere Ergebnis), oder
* **Wurf um 1 Stufe erhöhen** für diesen einen Wurf (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), oder
* **Umwandlung eines Misserfolgs in „Erfolg mit Kosten“** – die Aktion gelingt, aber der SL fügt sofort einen Preis hinzu (z.B. du verlierst Zeit, machst Lärm, verbrauchst eine Ressource, endest in einer schlechteren Position, ziehst Aufmerksamkeit auf dich, beschädigst Ausrüstung).

**Wiederherstellung von WdG:** zu Beginn der nächsten Sitzung kehrst du zum Limit zurück. Der SL kann **+1 WdG** für mutiges Risiko, großartige erzählerische Entscheidungen oder das Spielen von Konsequenzen gewähren.

* **Ausrüstung:** 1 „Schlüssel“-Werkzeug (z.B. Schwert, Gewehr, Hacker-Set), 1 Schutz (Rüstung, Energieschild, Tarnung), 3 Kleinigkeiten, die zum Konzept passen.

**Beispiel:** Spezialist: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>, G <span class="rpg-token token-d6">k6</span>. In Cyberpunk ist <span class="rpg-token token-stat">M</span> „Hacking/Einfluss“; in Fantasy ist <span class="rpg-token token-stat">M</span> „Magie/Wille“.



---

### 2) Wie man Aktionen auflö<span class="rpg-token token-math">st</span>


1. Der Spieler sagt **was er tut** und **wie** (Beschreibung in der Spielwelt).
2. Der Spielleiter legt die **Schwierigkeit** und den Einsatz fest („was bei einem Misserfolg passiert“).
3. Würfle mit dem Attributswurf (<span class="rpg-token token-stat">S</span>/W/G) und vergleiche mit der Schwierigkeit.

**Schwierigkeit (<span class="rpg-token token-stat">S</span>):**

* **3** leicht, **4** standard, **5** schwierig, **6** sehr schwierig, **8** heroisch, **12** legendär.

**Wurf-Ergebnis:**

* **1** – Misserfolg mit Konsequenz (eine Komplikation tritt definitiv ein).
* **< <span class="rpg-token token-stat">S</span>** – Misserfolg (aber die Szene geht weiter: Zeitverlust, Lärm, schlechtere Position, Verlust einer Ressource).
* **≥ <span class="rpg-token token-stat">S</span>** – Erfolg.
* **Maximal auf dem Würfel** (z.B. 12 auf <span class="rpg-token token-d12">k12</span>, 20 auf <span class="rpg-token token-d20">k20</span>) – außergewöhnlicher Erfolg: du erhältst einen zusätzlichen Vorteil.

**Modifikatoren ohne <span class="rpg-token token-stat">Z</span>ählen:**

* **Bessere Situation**: erhöhe den Würfel um 1 Stufe (<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>).
* **Schlechtere Situation**: senke den Würfel um 1 Stufe (<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>).
* **Hilfe eines Verbündeten** (kostet dessen Aktion): erhöhe den Würfel um 1 Stufe.

**Beispiel:** Der Adept versucht, ein Portal zu schließen (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>) bei Alarm und Stress → schlechtere Situation, fällt auf <span class="rpg-token token-d6">k6</span>. <span class="rpg-token token-stat">S</span> = 5. Wurf 6: Erfolg, aber der „Alarm“ bleibt im Hintergrund als erzählerischer Druck.



---

### 3) Bewegung und Kampf – standardmäßig ohne Raster, Raster als Option

**Standardmäßig: Theater des Geistes (empfohlen)**

* Entfernungen beschreiben als: **Nah** (in Reichweite), **Nicht weit** (einige Schritte), **Weit** (auf der anderen Seite der Bühne), **Sehr weit** (sniper/fahrzeugmäßig).
* In einer Runde hast du: **Bewegung + 1 Aktion**.

  * Bewegung verändert normalerweise die Entfernung um 1 „Grad“ (Nicht weit→Nah usw.).
* **Angriff**: Wurf **<span class="rpg-token token-stat">S</span>** (Nahkampf) oder **<span class="rpg-token token-stat">Z</span>** (Fernkampf) gegen die **Verteidigung** des Ziels.

**Verteidigung der Gegner (ungefähr):**

* **Schwach** 4, **Typisch** 5, **Elite** 6, **Boss** 8 (legendärer Boss 12).

**Folgen eines Treffers (schneller Kampf):**

* Ein Treffer verursacht **1 Herz**.
* Ein außergewöhnlicher Erfolg verursacht **2 Herzen** oder hat einen starken Effekt (Entwaffnen, Umwerfen, Ablenken).

**Deckung und Positionsvorteil:**

* Leichte Deckung / schlechterer Winkel: senke den Würfel des Angreifers um 1 Grad.
* Gute Position / Überraschung: erhöhe den Würfel um 1 Grad.

**Option: Spiel auf Raster**

* 1 Feld = 1–2 m. Bewegung in einer Runde: **bis zu 5 Felder**. Der Rest der Regeln bleibt unverändert.

**Beispiel:** Ein Spezialist schießt aus Deckung (<span class="rpg-token token-stat">Z</span> w12) auf eine Elite (Verteidigung 6). Das Ziel ist in leichter Deckung → <span class="rpg-token token-stat">Z</span> sinkt auf w8. Wurf 7: Erfolg, 1 Herz Schaden.



---

### 4) <span class="rpg-token token-stat">M</span>ächte, „Zauber“ und spezielle Aktionen (universell)


    Dies umfasst Magie, Psionik, Cybernetik, Gadgets, Filmtricks – je nach Welt.

* Wenn du etwas **über das Standardmaß** machst: gib **1 Machtpunkt** aus und würfle **<span class="rpg-token token-stat">M</span>**.
* Bestimme die Effektstärke:

**<span class="rpg-token token-stat">M</span>ächtebenen (T / Kosten):**

* **Trick** (kurzer Effekt, Trick, „Flash“): **T 4 / 0–1 MP**
* **Standard** (Angriff, Schild, Impuls, feine Kontrolle): **T 5 / 1 MP**
* **Stark** (Bereich, Heilung, Lähmung, Live-Hack): **T 6 / 2 MP**
* **Groß** (Szene ändern, mächtiger Eingriff): **T 8–12 / 3 MP**

**Misserfolg:** MP gehen verloren, und die Konsequenz ist sofort (Überlastung, digitaler Fußabdruck, Riss im Ritual, unerwünschte Aufmerksamkeit).

**Wiederherstellung:** Nach der Konfliktszene erhältst du **1 MP** zurück, nach einer sicheren Ruhepause – bis zur vollen Menge.

**Beispiel:** In einer Weltraumoper versucht ein Adept, den „Sensor“ eines Drohnen zu „verbiegen“: Standard, T 5, Kosten 1 MP. Wurf <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span> = 8: außergewöhnlicher Erfolg – die Drohne verliert das Signal und verwirrt die Spur.



---

### 5) Sturz, Risiko und Heilung

* Wenn du auf **0 Herzen** fällst, bist du **aus dem Spiel genommen** (verwundet, betäubt, im Schock – gemäß der Konvention).
* Ein Verbündeter kann eine Aktion verwenden, um dich auf **1 Herz** zu bringen (Erste Hilfe, Adrenalin, Systemneustart).
* Nach der Szene, wenn ihr einen Moment der Ruhe habt: Ihr kehrt zu **vollen Herzen** zurück, sofern die Bedingungen stimmen (Unterkunft, Verband, Wartung, Mahlzeit).
* Wenn die Szene besonders brutal war oder die Feinde im Vorteil sind, kann der Spielleiter verlangen, dass ein „voller Reset“ einen sicheren Halt erfordert.

**Beispiel:** Sturm fällt auf 0. Der Spezialist zieht ihn hinter Deckung und verwendet eine Aktion: Sturm kehrt auf 1 Herz zurück und kann in der nächsten Runde handeln.



---

### 6) Charakterentwicklung (Kampagne ohne Tabellen und Buchhaltung)


Po przygodzie wybierz **jedno**:

* **Verbessere** eine Eigenschaft um 1 Punkt (max. bis <span class="rpg-token token-d20">k20</span>), oder
* **+1 Herz** (max. 7), oder
* **+1 Kraftpunkt** (max. 5), oder
* **Neuer Vorteil** (kurze, einzeilige Regel, die mit dem Spielleiter abgestimmt ist).

**Beispiele für Vorteile (universell):**

* **Druck:** einmal pro Szene, wenn du im Nahkampf triffst, fügst du +1 Herz Schaden hinzu.
* **Schatten:** wenn du heimlich handelst, hast du einen Würfelbonus von 1 Punkt.
* **Funke:** einmal pro Szene kannst du 1 <span class="rpg-token token-math">KP</span> ausgeben, um automatisch „Erfolg mit Kosten“ ohne Würfelwurf zu erzielen.

**Beispiel:** Der Adept verbessert <span class="rpg-token token-stat">M</span> von <span class="rpg-token token-d8">k8</span> auf <span class="rpg-token token-d12">k12</span> – jetzt treten seine Kräfte stabiler bei T 5–6 auf.



---

### 7) Variante „nur <span class="rpg-token token-d6">k6</span>” im **2k6** Modus (schnell und sehr spielbar)


Falls ihr kein Würfelsatz habt oder eine „narrativere” Ergebnisstufen wünscht:

* Jeder Test ist: **würfle 2k6 + Attributmodifikator**.
* **Attributmodifikatoren** wählt zu Beginn: ein Attribut **+2**, eines **+1**, eines **+0**.
* Ergebnis:

  * **6 oder weniger** – Misserfolg mit Konsequenz
  * **7–9** – Erfolg mit Kosten (Kompromiss, Verlust eines Ressourcen, schlechtere Position)
  * **10+** – voller Erfolg
  * **12** – außergewöhnlicher Erfolg (zusätzlicher Vorteil)

**Schwierigkeitsgrad der Situation:** anstatt die Schwellenwerte zu ändern, gib **+1 / -1** zum Wurf (unterstützt / hindert) oder Kosten im Falle von 7–9.

**Mapping zur Würfel-Attribut-Version (wenn du Konsistenz möchtest):**

* <span class="rpg-token token-d6">k6</span> ≈ +0, <span class="rpg-token token-d8">k8</span> ≈ +1, <span class="rpg-token token-d12">k12</span> ≈ +2, <span class="rpg-token token-d20">k20</span> ≈ +3 (für sehr erfahrene Charaktere).

**Beispiel:** Spezialist schießt im Lauf: <span class="rpg-token token-stat">Z</span> = +2, schwierige Situation (-1). Wurf 2k6 = 8, Summe 9: Erfolg mit Kosten – trifft, endet aber in einer offenen Position.

