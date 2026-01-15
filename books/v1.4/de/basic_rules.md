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
generated_at: "2026-01-15T08:02:46.258Z"
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
# Grundregelwerk



---



---

### Benötigte Dinge für das Spiel

- Bleistift und Charakterbogen.
- (Optional) Karte/Gitter und Figurenmarker (kariertes Papier, Matte, VTT).
- Würfel: **<span class="rpg-token token-d4">k4</span>, <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-d20">k20</span>**.
  - In der Praxis reicht **je einer** von jedem (man würfelt immer mit einem Würfel gleichzeitig).
  - (Optional) **k100** für Zufallstabellen oder Generatoren.
- Wenn ihr nur **<span class="rpg-token token-d6">k6</span>** habt, verwendet die Variante **2k6** (am Ende).

---



---

### Glossar


Diese Wörter erscheinen in den Regeln — hier werden sie „menschlich“ erklärt:

- **SL (Spielleiter)**: leitet die Welt, beschreibt Situationen, steuert Gegner, legt die Schwierigkeit und Konsequenzen fest.
- **Spieler**: beschreibt die Aktionen seiner Figur und führt Würfe aus.
- **Wurf**: ein Würfelwurf, der ein unsicheres Ergebnis entscheidet.
- **Eigenschaften**: **<span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>)**, **Geschicklichkeit (G)**, **Macht (<span class="rpg-token token-stat">M</span>)**. Sie sagen, *mit welchem Würfel du wirfst*.
- **Eigenschaftswurf**: die Größe des Würfels, der der Eigenschaft zugeordnet ist (z. B. G = W12).
- **Schwierigkeit (<span class="rpg-token token-stat">S</span>)**: die Zahl, die erreicht oder übertroffen werden muss, damit die Aktion gelingt.
- **Erfolg**: Ergebnis ≥ Schwierigkeit.
- **Besonderer Erfolg**: **maximales Ergebnis** auf dem Würfel (z. B. 12 auf W12, 20 auf W20) — Erfolg + zusätzlicher Vorteil.
- **Komplikation**: zusätzliches Problem nach einem Misserfolg (Lärm, Zeitverlust, schlechtere Position, Verlust einer Ressource).
- **Erfolg mit Kosten**: die Aktion gelingt, aber du zahlst einen Preis (Kompromiss, Verlust einer Ressource, Enthüllung, Risiko).
- **Glückswurf (GW)**: begrenzte Ressource, die es ermöglicht, Szenen zu retten (Wurf wiederholen / Würfel erhöhen / Misserfolg in Erfolg mit Kosten umwandeln).
- **Herzen**: „Leben“ der Figur (Ausdauer, Wunden, Zustand — je nach Welt).
- **Machtpunkte (MP)**: Ressource für Kräfte und „überstandardmäßige“ Aktionen (Magie, Psionik, Gadgets, „filmische“ Aktionen).
- **Verteidigung**: Treffergrenze für den Gegner im Kampf (anstatt die Regeln für Rüstung, Rüstungsstufen usw. zu multiplizieren).
- **Sichtschutz**: Hindernis zwischen dir und dem Ziel. Erschwert normalerweise Fernangriffe oder Beobachtungsaktionen.

---



---

### 1. Charakter


    Die Charaktererstellung ist kurz. Ein Charakter ist: **Konzept + Rolle + Eigenschaften + Ressourcen + Ausrüstung**.

---

### 1.1 Konzept

Ein Satz: Wer bist du und in welchem Genre spielst du.

> Beispiel: „Ehemalige Agentin einer Corporation, heute Kopfgeldjägerin, die im Verborgenen agiert und niemandem vertraut.”

### 1.2 Rolle (wähle eine)


Rollen sind absichtlich „weltneutral“. In Fantasy kannst du sie anders nennen, im Cyberpunk anders, aber sie funktionieren gleich.

- **Sturm** — Druck, Kampf, Überwinden von Hindernissen, Durchbrechen der Front.
- **Spezialist** — Schleichen, Präzision, Technik, Beobachtung, Plan.
- **Adept** — Kräfte, Einfluss, Wissen, Improvisation (Magie/Psionik/Technologie je nach Welt).


### 1.3 Eigenschaften und Würfel


Du hast drei Eigenschaften:

- **<span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>)** — physische Kraft, Ausdauer, Nahkampf, Durchsetzen.
- **Geschicklichkeit (G)** — Reflexe, Präzision, Schleichen, Schießen, Fahren.
- **Macht (<span class="rpg-token token-stat">M</span>)** — „das Besondere“: Magie, Psionik, fortgeschrittene Technologie, soziale Täuschung, Intuition — je nach Konvention.

**Zu Beginn verteile die Würfel so:**
- eine Eigenschaft hat **<span class="rpg-token token-d12">k12</span>**,
- eine hat **<span class="rpg-token token-d8">k8</span>**,
- eine hat **<span class="rpg-token token-d6">k6</span>**.

**Vorgeschlagene Verteilung nach Rolle (am einfachsten):**
- **Sturm:** <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>, G <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d6">k6</span>
- **Spezialist:** G <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>
- **Adept:** <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>, G <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>

> Beispiel: Wenn du G = <span class="rpg-token token-d12">k12</span> hast, würfelst du normalerweise <span class="rpg-token token-d12">k12</span> bei Schüssen, Schleichen und Ausweichmanövern.

### 1.4 Ressourcen

- **Herzen:** 5.
- **Machtpunkte (MP):** 3.
- **Glückswurf (GW):** zu Beginn jeder Sitzung hast du **2 GW**.

**Glückswurf (wie es funktioniert):** gib **1 GW** aus, um eines auszuwählen:
- **Wiederholung** deines Tests (du behältst das bessere Ergebnis), oder
- **Wurf um 1 Stufe erhöhen** für diesen einen Wurf (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), oder
- **Misserfolg in „Erfolg mit Kosten” umwandeln** — die Aktion gelingt, aber der Spielleiter fügt sofort einen Preis hinzu (z.B. Lärm, Zeitverlust, Verlust einer Ressource, schlechtere Position, Aufmerksamkeit erregen, Ausrüstungsschaden).

**Wiederherstellung von GW:** zu Beginn der nächsten Sitzung kehrst du zum Limit zurück. Der Spielleiter kann **+1 GW** für mutiges Risiko, großartige erzählerische Entscheidungen oder das Spielen von Konsequenzen gewähren.

### 1.5 Talente (optional, aber empfohlen)

Talente sind **2 kurze Schlagwörter**, die beschreiben, worin deine Figur gut ist (ohne Liste, ohne Tabelle).

- Beispiele: „Mechaniker“, „Späher“, „Verhandler“, „Heiler“, „Hacker“, „Veteran“, „Entdecker“.

**Wie Talente funktionieren:** Wenn ein Talent tatsächlich bei einem Test hilft, kann der SL **den Würfel um 1 Grad erhöhen** (oder eine Erschwernis neutralisieren).
- Ein Talent gewährt keine automatischen Erfolge.
- In der Regel beeinflusst **höchstens 1 Talent** einen Test.

### 1.6 Ausrüstung

Liste:
- 1 „schlüssel” Werkzeug (Waffe / Set / Ausrüstung, ohne die du deine Arbeit nicht machst),
- 1 Schutz (Rüstung, Schild, Tarnung — je nach Welt),
- 3 nützliche Kleinigkeiten für das Abenteuer.

Ausrüstung im Kern der Regeln ist hauptsächlich **eine Erlaubnis** (ermöglicht Aktionen) und kein numerischer Bonus.

### 1.7 Beispiel einer vollständigen Figur

- Konzept: „Informationsdiebin, die Daten aus Systemen stiehlt, nicht aus Taschen.”
- Rolle: Spezialist
- Eigenschaften: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>
- Ressourcen: 5 Herzen, 3 <span class="rpg-token token-power">PM</span>, 2 LP
- Talente: „Hacker”, „Schatten”
- Ausrüstung: Pistole, leichte Rüstung, Einbruchswerkzeug, Seil, Taschenlampe

---



---

### 2. Kern der Regeln: Tests

Dieser Teil ist der wichtigste — wenn du ihn verstehst, verstehst du das System.

### 2.1 Wann machst du einen Test


Ein Test wird durchgeführt, wenn beide Bedingungen erfüllt sind:
1) Das Ergebnis ist ungewiss (es könnte gelingen oder nicht), und
2) Der Einsatz ist real (ein Misserfolg ändert etwas / kostet etwas).

Wenn die Handlung banal und ohne Druck ist — kann der SL sagen „es ist gelungen“ ohne einen Wurf.

### 2.2 Wie man einen Test durchführt (Schritt für Schritt)

1) Der Spieler sagt **was er tut** und **warum**.
2) Der Spielleiter wählt eine Eigenschaft: **<span class="rpg-token token-stat">S</span>** oder **<span class="rpg-token token-stat">Z</span>** oder **<span class="rpg-token token-stat">M</span>**.
3) Der Spielleiter legt die **Schwierigkeit (<span class="rpg-token token-stat">S</span>)** fest und erklärt, was ein Misserfolg bedeutet (Einsatz).
4) Der Spieler würfelt mit dem **Eigenschaftswurf**.
5) Vergleiche das Ergebnis mit der <span class="rpg-token token-stat">S</span> und bestimme die Folgen.

### 2.3 Schwierigkeiten (T)


Wir verwenden einfache Schwellenwerte. Wenn du dir unsicher bist – wähle einen niedrigeren Schwellenwert, und die „Schwierigkeit“ zeigt sich in den Konsequenzen.

- **T 3** – einfach (fast sicher, aber manchmal lohnt es sich, unter Druck zu überprüfen)
- **T 4** – standard (typische Herausforderung)
- **T 5** – schwierig (erfordert Kompetenz oder Vorteil)
- **T 6** – sehr schwierig (ohne Vorteil ist es riskant)
- **T 8** – heroisch (für die Besten oder nach guter Vorbereitung)
- **T 12** – legendär (selten „rein“; normalerweise als Kampagnenziel, Plan, Ritual, große Bedingungen)

### 2.4 Testergebnisse

- **Ergebnis ≥ T → Erfolg.** Du erzielst den gewünschten Effekt.
- **Ergebnis < T → Misserfolg.** Du erzielst den Effekt nicht, und die Situation ändert sich (Komplikation oder Kosten).
- **Wurf 1 → Misserfolg + Komplikation.** Eine Komplikation tritt auf jeden Fall ein.
- **Maximaler Wurf auf dem Würfel → Außergewöhnlicher Erfolg.**
  - Neben dem Erfolg erhältst du **einen zusätzlichen Vorteil** (schneller, leiser, <span class="rpg-token token-math">st</span>ärker, sicherer, zusätzlicher Effekt).

> Beispiel für einen Erfolg mit Kosten: „Es ist dir gelungen, die Tür zu überwinden, aber du machst Lärm und jemand kommt, um nachzusehen.“

### 2.5 Erleichterungen und Erschwernisse (ohne <span class="rpg-token token-stat">Z</span>ählen)


Statt +1/−1 zu Würfen hinzuzufügen, ändern wir die **Würfelgröße**.

- **Bessere Situation** → **steigere den Würfel um 1 Stufe**  
  <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **Schlechtere Situation** → **senke den Würfel um 1 Stufe**  
  <span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**Beispiele für Erleichterungen:** Vorbereitung, gute Werkzeuge, Positionsvorteil, Überraschung, Unterstützung.  
**Beispiele für Erschwernisse:** Dunkelheit, Glätte, Zeitdruck, Lärm, Ablenkung, Deckung.

**Regel der Ordnung:** Für die Schnelligkeit gehe davon aus, dass ihr in einem Test normalerweise **maximal 1 Erleichterung und 1 Erschwernis** anwendet (sie können sich gegenseitig aufheben).

### 2.6 Hilfe eines Verbündeten

Ein Verbündeter kann seine Aktion (oder Zeit in einer Szene außerhalb des Kampfes) opfern, um zu helfen.

**Effekt:** für diesen einen Wurf **erhöhe den Würfel um 1 Stufe**.

Die Hilfe muss sinnvoll beschrieben werden (Schutz bieten, Werkzeuge reichen, Ablenkung erzeugen, Stabilisierung, Hinweise geben).

### 2.7 Wiederholung von Tests


Wenn der Test nicht bestanden wurde, wiederhole ihn nicht „endlos“, ohne die Situation zu ändern.
- Entweder machst du etwas anders (eine andere Eigenschaft / andere Werkzeuge / einen anderen Weg),
- oder du akzeptierst die Kosten (Zeit, Alarm, Ressource),
- oder du ziehst dich zurück.

### 2.8 Beispiele für Tests (außerhalb des Kampfes)

**Beispiel A — leise Überquerung**
- Spieler: „Ich gehe über den Hof, bevor der Scheinwerfer zurückkommt.“
- SL: Geschicklichkeit (G). Das steht unter Zeitdruck → Schwierigkeit **<span class="rpg-token token-stat">S</span> 5**.
- Die Figur hat das Talent „Schatten“ → Erleichterung, Würfel um 1 Grad erhöht.
- Wurf: W12 = 4 → Misserfolg. SL: „Sie bemerken dich nicht sofort, aber jemand hört ein Rascheln und beginnt, das Gelände zu überprüfen (Komplikation: der Druck steigt)."

**Beispiel B — gewaltsames Aufbrechen**
- Spieler: „Ich breche die Metalltür auf, bevor die Wache um die Ecke kommt.“
- SL: <span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>), Schwierigkeit **<span class="rpg-token token-stat">S</span> 6** (sehr schwierig ohne Werkzeuge).
- Jemand hilft, indem er das Schloss festhält und die Tür klemmt → Würfel um 1 Grad erhöht.
- Wurf: <span class="rpg-token token-stat">S</span> W12 = 12 → außergewöhnlicher Erfolg: Die Tür öffnet sich sofort und du machst es leiser, als erwartet.



---

### 3. Bewegung und Entfernungen (Gitter ist optional)

Standardmäßig funktioniert NDE ohne Karte: Du beschreibst die Szene und die Positionen der Charaktere.

### 3.1 Standardmäßig: beschreibende Entfernungen


Verwende vier Zonen:
- **Nah** — zum Greifen nah, Nahkampf.
- **In der Nähe** — einige Schritte, leichter Zugriff.
- **Weit** — andere Seite der Szene, erfordert deutliches Bewegen.
- **Sehr weit** — scharfschützenmäßig/Fahrzeugmäßig/„an der Grenze der Szene“.

In einer Runde kannst du normalerweise die Entfernung um **eine Zone** ändern (z.B. Weit → In der Nähe).

### 3.2 Option: Spiel auf dem Gitter (für Taktik)


Wenn ihr Konkretes bevorzugt:
- 1 Feld = 1–2 m.
- Bewegung in einer Runde: **bis zu 5 Felder**.
- Diagonalen sind erlaubt (zählen wie ein normales Feld).


### 3.3 Deckung und Aktionslinie

- **Vollständige Deckung:** Es ist nicht möglich, „geradeaus“ zu interagieren (Schuss, Beobachtung, viele Kräfte).
- **Teilweise Deckung:** Erschwert — normalerweise **senkt den Würfel um 1 Stufe** für den angreifenden/beobachtenden.



---

### 4. Kampf

Kampf ist eine gewöhnliche Szene mit Tests, nur in Runden geordnet.

### 4.1 Wann beginnt der Kampf


Der Kampf beginnt, wenn:
- mindestens eine Seite die andere verletzen möchte, und
- es wichtig ist, wer und wann handelt.

Wenn die Situation kurz und offensichtlich ist, kann der Spielleiter sie mit einem einzigen Wurf entscheiden.

### 4.2 Reihenfolge der Runden (einfache Version)


Am einfachsten:
- Zuerst handeln alle Spieler (in beliebiger Reihenfolge),
- dann handeln die Gegner,
- und so weiter in einer Schleife.

### 4.3 Was tust in deinem Zug


In deinem Zug hast du:
- **Bewegung** (Wechsel der Zone / bis zu 5 Felder im Raster-Variante),
- **1 Aktion** (Angriff, Test, Hilfe, Einsatz von Kräften, Ausrüstung, Interaktion mit der Szene).


### 4.4 Angriff: wie es funktioniert

1) Wähle ein Ziel und beschreibe den Angriff.
2) Wähle eine Eigenschaft:
   - **Nahkampf** → Würfel **<span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>)**,
   - **Fernkampf** → Würfel **Geschicklichkeit (G)**,
   - **<span class="rpg-token token-stat">M</span>ächte** → normalerweise Würfel **Macht (<span class="rpg-token token-stat">M</span>)** (siehe Kapitel 5).
3) Bestimme die **Rüstung** des Ziels.
4) Würfle und vergleiche mit der Rüstung.

### 4.6 Schäden und „wie viel sie aushalten”


- Ein Treffer verursacht **1 Herz**.
- **Außergewöhnlicher Erfolg** verursacht **2 Herzen** *oder* hat einen starken Effekt (Entwaffnung, Umwerfen, Herausdrängen aus der Deckung) — wähle eines.

Einfachste Archetypen von Gegnern:
- **Handlanger:** fällt nach 1 Treffer aus.
- **Elite:** hat **2 Herzen**.
- **Boss:** hat **3 Herzen** (oder 5 in finalen Szenen).

> Hinweis: „ausfallen” muss nicht den Tod bedeuten. Er kann ohnmächtig sein, geflohen sein, sich ergeben haben oder aus dem Geschehen entfernt worden sein.

### 4.5 Verteidigung der Gegner (orientierend)

- **Schwach:** Verteidigung **4**
- **Typisch:** Verteidigung **5**
- **Elite:** Verteidigung **6**
- **Boss:** Verteidigung **8** (legendärer Boss: **12**)

Schutz und Bedingungen ändern normalerweise die Größe der Würfel des Angreifers (Erleichterungen/Erschwernisse) und nicht die Verteidigung.

### 5.7 Reichweite der Angriffe (Standard)
Um die Zahlen nicht zu vervielfachen, benutze einfache Regeln:
- Nah: Ziel auf dem benachbarten Feld.
- Distanz: Ziel in „Sichtweite” auf dem Spielfeld.
  - Wenn der Spielleiter Einschränkungen möchte: akzeptiere **bis zu 10 Felder** ohne Strafe; über 10 Felder <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> +1 Grad.

### 5.8 Mehrere Gegner gleichzeitig
Wenn mehrere Gegner „im Nahkampf” mit einer Figur sind, kann der Spielleiter:
- den Schwierigkeitsgrad um 1 erhöhen (Druck), oder
- die Niederlage als zusätzliche Komplikation werten (z.B. du verlierst deine Position).

Die Regel soll schnell sein: **eine Entscheidung → ein Effekt**.

### 4.7 Beispiele für Kämpfe

**Beispiel A — Nahkampf mit einem Wachmann**
- Sturm (<span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>) greift den Wachmann (Verteidigung 5) an.
- Die Bedingungen sind günstig (Überraschung) → Würfel wird um 1 Stufe erhöht, aber es ist bereits <span class="rpg-token token-d12">k12</span>, also wird er auf <span class="rpg-token token-d20">k20</span> erhöht.
- Wurf <span class="rpg-token token-d20">k20</span> = 7 → Treffer, der Wachmann fällt aus.

**Beispiel B — Schuss auf die Elite aus Deckung**
- Spezialist (<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>) schießt auf die Elite (Verteidigung 6).
- Das Ziel ist teilweise in Deckung → Erschwernis, der Würfel fällt auf <span class="rpg-token token-d8">k8</span>.
- Wurf <span class="rpg-token token-d8">k8</span> = 6 → Treffer, die Elite verliert 1 Herz (hat noch 1).

**Beispiel C — Boss und Glücksgriff**
- Adept (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>) versucht, den Boss (Verteidigung 8) mit Macht zu überwältigen.
- Wurf <span class="rpg-token token-d12">k12</span> = 4 → Misserfolg. Der Spieler gibt 1 Glückspunkt für einen Nachwurf aus.
- Nachwurf = 10 → Erfolg. Der Boss verliert 1 Herz, aber der SL fügt die Kosten hinzu: „Der Effekt ist laut, der Alarm geht los.”



---

### 5. <span class="rpg-token token-stat">M</span>ächte (<span class="rpg-token token-stat">M</span>) und Machtpunkte (MP)

In NDE ist „Macht“ eine Kategorie von Spezialeffekten. Je nach Welt kann dies bedeuten:
- Magie, Psionik, Rituale,
- fortschrittliche Technologie, Drohnen, Live-Hacking,
- filmische Aktionen von Helden (z.B. „meisterhafte Konzentration“),
- sozialen Einfluss in Spielen, wo das Gespräch „Macht“ ist.

### 5.1 Wann du <span class="rpg-token token-power">PM</span> ausgibst

Du gibst <span class="rpg-token token-power">PM</span> aus, wenn du versuchst, einen **über den Standard hinausgehenden** Effekt zu erzielen.

---

### 5.2 Wie man Macht verwendet (Schritt für Schritt)

1) Beschreibe den Effekt, den du erzielen möchtest.
2) Der SL legt die Schwierigkeit und die Kosten in <span class="rpg-token token-power">PM</span> fest.
3) Gib <span class="rpg-token token-power">PM</span> aus.
4) Würfle **<span class="rpg-token token-stat">M</span>** und vergleiche mit der Schwierigkeit.

**Misserfolg:** Der Effekt funktioniert nicht; <span class="rpg-token token-power">PM</span> gehen verloren; es tritt eine Komplikation auf (Überlastung, Spur, Offenbarung, Nebenwirkung).

### 5.3 Effektstufen (Schwierigkeit / Kosten)

- **Trick** (kurzer Trick): **T 4 / 0–1 <span class="rpg-token token-power">PM</span>**  
  Licht, Geräusch, kleine Illusion, kurzfristige Ablenkung.
- **Standard**: **T 5 / 1 <span class="rpg-token token-power">PM</span>**  
  Geschoss, Schild, Impuls, Sprung, Verstärkung.
- **Stark**: **T 6 / 2 <span class="rpg-token token-power">PM</span>**  
  Bereich, Kontrolle, Heilung, Lähmung, „Hack im Kampf“.
- **Groß**: **T 8–12 / 3 <span class="rpg-token token-power">PM</span>**  
  Effekt, der die Szene verändert oder kampagnenrelevante Konsequenzen hat.

### 5.4 Außergewöhnlicher Erfolg in der Macht


Wenn du das Maximum auf dem Wurf mit dem W6 erzielst:
- erhöhe den Maßstab (größeres Gebiet / länger / <span class="rpg-token token-math">st</span>ärker), oder
- füge einen zusätzlichen Vorteil hinzu (leiser, präziser, sicherer), oder
- der SL kann **1 <span class="rpg-token token-power">PM</span>** zurückgeben (wenn es zur Fiktion passt).


### 5.5 Wiederherstellung von <span class="rpg-token token-power">PM</span>

- Nach einer Konfliktszene erhältst du **1 <span class="rpg-token token-power">PM</span>**.
- Nach einem sicheren Ruhetag kehrst du zu voller Gesundheit zurück.

### 5.6 Beispiele für Kräfte

**Beispiel A — Schild zum Laufen**
- Spieler: „Ich stelle ein kurzes Schild auf, um zu einer besseren Position zu laufen.“
- SL: Standard **T 5**, Kosten 1 <span class="rpg-token token-power">PM</span>.
- Wurf <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span> = 9 → Erfolg: Du läufst sicher vorbei.

**Beispiel B — Misserfolg mit Konsequenz**
- Spieler: „Ich halte die Elite an Ort und Stelle.“
- SL: Starke **T 6**, Kosten 2 <span class="rpg-token token-power">PM</span>.
- Wurf = 1 → Misserfolg + Komplikation: Du verlierst 2 <span class="rpg-token token-power">PM</span>, und der Effekt prallt zurück und verrät deine Position.



---

### 6.1 0 Herzen

Wenn du auf 0 Herzen fällst:
- bist du **aus dem Spiel genommen** (verwundet, betäubt, im Schock – je nach Konvention),
- kann ein Verbündeter eine Aktion opfern, um dich mit **1 Herzen** wieder auf die Beine zu bringen.

### 6.2 Ruhe

- Nach einer Konfliktszene, wenn ihr einen Moment der Ruhe und die grundlegenden Bedingungen habt, könnt ihr zu vollen Herzen zurückkehren.
- In strengeren Kampagnen kann der Spielleiter einen sicheren Halt verlangen, um zur Vollständigkeit zurückzukehren.

---

### 7.3 Ruhe
Nach einer Kampfszene oder einem Konflikt, wenn ihr einen Moment sicheren Ruhe (und grundlegende Bedingungen) habt, kehrt ihr zu voller <span class="rpg-token token-math">St</span>ärke zurück:
- Herzen,
- Mana.

Dies hält das System schnell und erfordert keine langen Heilungszeiten.



---

### 7. Charakterentwicklung

**Wenn du wächst:** nach einem Abenteuer, einer Mission oder einem wichtigen Kapitel der Handlung (normalerweise alle 1–3 Sitzungen).

Wähle **eine** Option:
- **Erhöhe** eine Eigenschaft um 1 Würfelstufe (max. bis <span class="rpg-token token-d20">k20</span>), oder
- **+1 Herz** (max. 7), oder
- **+1 MP** (max. 5), oder
- **Neues Merkmal** (eine Satz, spezifische Fähigkeit, die mit dem SL vereinbart wurde).

> Beispiel: Der Spezialist erhöht <span class="rpg-token token-stat">Z</span> von <span class="rpg-token token-d12">k12</span> auf <span class="rpg-token token-d20">k20</span>, weil die Kampagne in die Phase von Verfolgungsjagden und Schießereien übergegangen ist.

---



---

### 8. Variante nur <span class="rpg-token token-d6">k6</span>: 2k6

Wenn ihr keine verschiedenen Würfel verwenden wollt, spielt mit **2k6**.

### 8.1 Eigenschaften als Modifikatoren


Statt der Würfelgrößen teile die Modifikatoren auf:
- Eine Eigenschaft hat **+2**
- Eine hat **+1**
- Eine hat **+0**


### 8.2 Test

Würfle **2W6 + Attributmodifikator**.

**Ergebnis:**
- **6 oder weniger** – Misserfolg mit Konsequenz
- **7–9** – Erfolg mit Kosten
- **10+** – voller Erfolg
- **12** – außergewöhnlicher Erfolg (zusätzlicher Vorteil)

### 8.3 Schwierigkeit der Situation


Statt die Schwellenwerte zu ändern, gib:
- **+1** für Vorteil, Vorbereitung, guten Plan,
- **−1** für Hindernisse, Druck, Deckung, Chaos.

### 8.4 Glücksgriff in 2k6

Gib 1 Glückspunkt aus, um:
- 2k6 neu zu würfeln, oder
- **+1** zum Ergebnis des Tests hinzuzufügen, oder
- einen Misserfolg gegen einen Erfolg mit Kosten zu tauschen.

### 8.5 Schnelles Mapping (optional)

Wenn du irgendwann einen Charakter zwischen den Varianten "umrechnen" möchtest:
- <span class="rpg-token token-d6">k6</span> ≈ +0
- <span class="rpg-token token-d8">k8</span> ≈ +1
- <span class="rpg-token token-d12">k12</span> ≈ +2
- <span class="rpg-token token-d20">k20</span> ≈ +3 (für sehr erfahrene)



---

[DE] Platzhalter für Inhalt...




---

### 1. Einleitung

7.2 Diese Ergänzungen sind nicht erforderlich, können aber manchmal die Durchführung erleichtern.

### 9.1 Schutz (Rüstung) als einfacher Ressource


Wenn du möchtest, dass „Schutz“ einen deutlichen Effekt hat:
- Eine Figur mit Schutz hat **1 Rüstungsmarker pro Szene**,
- wenn sie 1 Herz verlieren würde, kann sie stattdessen einen Rüstungsmarker verwenden.

### 9.2 Zeitdruck als Timer

Wenn die Szene ein Zeitlimit hat, legt der SL einen „<span class="rpg-token token-stat">Z</span>ähler“ fest (z. B. 3 Schritte). Jeder Misserfolg verschiebt den <span class="rpg-token token-stat">Z</span>ähler um 1. Wenn das Ende erreicht ist — tritt eine Konsequenz ein (Alarm, Flucht des Ziels, Einsturz des Durchgangs).

---

### 9.3 Vergeltung (Variante des riskanten Kampfes)

Wenn du möchtest, dass der Kampf „härter“ und schneller ist:
- wenn du **im Nahkampf angreifst** und **verfehlst**, verlierst du **1 Herz**, es sei denn, der Gegner konnte dich tatsächlich erreichen.
Das ist eine Variante — im Kern von NDE ergeben sich die Konsequenzen von Misserfolgen im Kampf hauptsächlich aus der Fiktion und den Entscheidungen des SL.

