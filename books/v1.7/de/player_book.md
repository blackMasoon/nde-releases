---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.7
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
generated_at: "2026-01-16T10:17:16.377Z"
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
# Spielerhandbuch

Automatic translation placeholder for de

---



---

### 1) Wie das Spiel am Tisch aussieht

- **Spielleiter (SL)** beschreibt die Situation und sagt, was in dieser Szene möglich ist.
- **Du** sagst: **was du machst** und **welchen Effekt du erzielen möchtest.**
- Wenn das Ergebnis unsicher oder riskant ist, sagt der SL:
  1) **welches Attribut** du verwendest (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>),
  2) **wie groß die Schwierigkeit** <span class="rpg-token token-t">T</span> ist (oder **die Verteidigung** des Ziels),
  3) **was bei einem Misserfolg droht** (Konsequenz).

Dann würfelst du den Attributswürfel und ihr wisst sofort, was als Nächstes passiert.

### Die kürzeste Regel

**Würfle einen Eigenschaftswürfel. Ergebnis ≥ <span class="rpg-token token-t">T</span> = Erfolg.**



---

### 2) Was hat dein Charakter

Dein Charakter hat: - **Konzept** (1 Satz: wer du bist, in welcher Welt du agierst), - **Rolle** (Sturm / Spezialist / Adept), - 3 **Eigenschaften**: <span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>), Geschicklichkeit (<span class="rpg-token token-stat">Z</span>), Macht (<span class="rpg-token token-stat">M</span>), - **Herzen** (Ausdauer) und **Machtpunkte** (MP), - **Glückssträhne** (GS), - (optional) **Talente**, - **Ausrüstung**.

### 2.1 Eigenschaften (K/G/<span class="rpg-token token-stat">M</span>) — wofür sie gut sind

- **Kraft (K)**: Nahkampf, Erzwingen, Tragen, Ausdauer.
- **Geschicklichkeit (G)**: Schießen, Präzision, Schleichen, Ausweichen, Akrobatik, Fahren von Fahrzeugen.
- **Macht (<span class="rpg-token token-stat">M</span>)**: „Spezialeffekte“ der Spielwelt: Magie, Psionik, Glaube, Supertechnologie, Hacking, Einfluss, Intuition — abhängig von der Konvention.

### 2.2 Eigenschaftswürfel — wie sie funktionieren

Jede Eigenschaft hat einen Würfel: <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>, <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> oder <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>.  
Wenn du eine Eigenschaft benutzt, wirfst du **einen Würfel** dieser Eigenschaft.

- Größerer Würfel = höhere Chance auf Erfolg und auf außergewöhnlichen Erfolg (Maximalwert auf dem Würfel).

**Beispiel:** Du hast Geschicklichkeit <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>. Wenn du schießt, kletterst oder schleichst, würfelst du normalerweise <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>.

### 2.3 Ressourcen: Herzen, Machtpunkte und Glückspunkte

- **Herzen:** 5 am Anfang. Treffer und Druck nehmen Herzen weg.
- **Machtpunkte (MP):** 3 am Anfang. Du gibst sie für Kräfte und überdurchschnittliche Aktionen aus.
- **Glückspunkte (GP):** 2 am Anfang jeder Sitzung. Das ist dein „Szenenretten“ und der Dreh an der Dramatik.



---

### Schritt 1: Konzept und Rolle

Wähle eine Rolle – dies ist der allgemeine Handlungsstil (passt in jedes Universum).

- **Sturmangriff**: Du gehst Risiken ein und treibst Szenen voran.  
  (z.B. Krieger, Marines, Wachmann, Jäger, Barbar)
- **Spezialist**: Du handelst präzise, mit Plan und Werkzeugen.  
  (z.B. Schurke, Scharfschütze, Kundschafter, Hacker, Pilot, Fährtenleser)
- **Adept**: Du tust Dinge „über dem Standard“ – mit Macht, Wissen, Einfluss.  
  (z.B. Magier, Psioniker, Priester, Alchemist, Technomant, Diplomat)

### Schritt 2: Verteile Attributswürfel

Verteile die Würfel: ein Attribut <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>">w12</span>, ein <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>">w8</span>, ein <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>">w6</span>.

Schnelle Hinweise:
- **<span class="rpg-token token-math">St</span>ürmer** hat normalerweise K am höchsten.
- **Spezialist** hat normalerweise T am höchsten.
- **Adept** hat normalerweise <span class="rpg-token token-stat">M</span> am höchsten.

### Schritt 3: Ressourcen notieren

- **Herzen:** 5  
- **Kraftpunkte:** 3  
- **Glückspunkt:** 2 (zu Beginn der Sitzung erneuert)

### Schritt 4 (optional): Wähle 2 Talente

Talente sind kurze Bezeichnungen, die beschreiben, worin du gut bist (Kompetenzen, die im Spiel oft wiederkehren).
- Beispiele: „Kundschafter“, „Mechaniker“, „Mediziner“, „Verhandlungsexperte“, „Athlet“, „Analytiker“, „Hacker“, „Ritualist“.

**Wie Talente funktionieren:** Wenn ein Talent den Test tatsächlich unterstützt, betrachtet der Spielleiter dies als verbesserte Situation und du kannst den **Würfel um 1 Stufe erhöhen** für diesen Wurf.  
- Normalerweise 1 Talent pro Test.
- Ein Talent ersetzt nicht die Beschreibung des Handelns – es soll einen sinnvollen Plan verstärken.

**Beispiel:** Du hast das Talent „Mechaniker“ und versuchst, einen Generator notfallmäßig zu starten. Der Spielleiter erkennt an, dass dies hilft: Du erhöhst <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> auf <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> für diesen Test.

### Schritt 5: Ausrüstung

Notiere:
- 1 „Schlüssel“-Werkzeug (Waffe oder Berufsausrüstung),
- 1 Schutz (Rüstung, Schild, Tarnung – je nach Welt),
- 3 Gebrauchsgegenstände.

Ausrüstung funktioniert meist als **Berechtigung**: Wenn du etwas hast, kannst du versuchen, die entsprechenden Aktionen durchzuführen. Ein gutes Werkzeug kann auch eine bessere Situation schaffen (Würfelvorteil), wenn es sinnvoll ist.

### Beispielcharakter (universal)

- Rolle: Spezialist  
- <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, G <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>  
- Herzen 5, MP 3, GS 2  
- Talente: „Späher“, „Verhandlungsführer“  
- Ausrüstung: Fernkampfwaffe, Dietriche / Werkzeugsatz, Seil, Taschenlampe





---

### 4.1 Wann du wirfst

Du würfelst, wenn:
- etwas **riskant** oder unsicher ist,
- ein Fehlschlag **bedeutende Konsequenzen** hat.

Wenn etwas offensichtlich und ohne Druck ist, kann der Spielleiter sagen „es gelingt“ ohne einen Wurf.

### 4.2 Schwierigkeit <span class="rpg-token token-t">T</span>

Der Spielleiter wählt die Schwierigkeit:

- <span class="rpg-token token-t">T 3</span> leicht  
- <span class="rpg-token token-t">T 4</span> standard  
- <span class="rpg-token token-t">T 5</span> schwierig  
- <span class="rpg-token token-t">T 6</span> sehr schwierig  
- <span class="rpg-token token-t">T 8</span> heroisch  
- <span class="rpg-token token-t">T 12</span> legendär

Du musst die Schwierigkeit nicht „erraten“ — der Spielleiter sagt sie direkt.

### 4.3 Wurfergebnisse

- **1**: Misserfolg mit Konsequenz (eine Komplikation tritt definitiv ein). 
- **Ergebnis < <span class="rpg-token token-t">T</span>**: Misserfolg (aber die Szene geht weiter).
- **Ergebnis ≥ <span class="rpg-token token-t">T</span>**: Erfolg.
- **Max auf dem Würfel** (z.B. 12 auf <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, 20 auf <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>): außergewöhnlicher Erfolg + zusätzlicher Vorteil.

**Zusätzlicher Vorteil** (Beispiele): schneller, leiser, sicherer, größerer Effekt, bessere Position, zusätzlicher Detailvorteil für dich.

### 4.4 Bessere/schlechtere Situation (ohne Boni)

Statt Modifikatoren zu zählen, spielt ihr die Situation aus:

- **Bessere Situation** → Erhöhe den Würfel um 1 Stufe  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>)
- **Schlechtere Situation** → Verringere den Würfel um 1 Stufe  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>)

Deine Rolle als Spieler: **erschaffe bessere Bedingungen** durch Beschreibung und Entscheidungen (Deckung, Vorbereitung, Werkzeuge, Plan, Erkundung).

### 4.5 Hilfe des Verbündeten

Ein Verbündeter kann seine Aktion nutzen, um dir zu helfen. Dann, für diesen einen Wurf:
- Erhöhst du den Würfel um 1 Grad.

Die Hilfe muss im Kontext Sinn ergeben (Ablenkung, Deckung, Übergabe von Werkzeugen, Feuerunterstützung, ein zweites Paar Hände).

### Testbeispiel (klar und vollständig)

Du möchtest eine verschlossene Tür öffnen, bevor die Wachen kommen.
- SL: „Das ist Geschicklichkeit. <span class="rpg-token token-t">T 5</span>. Scheitern: Du machst Lärm und verlierst Zeit.“
- Du hast G <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, aber du benutzt Dietriche und hast das Talent „Schloss-Spezialist“ → bessere Situation, du würfelst mit <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.
- Wurf <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> = 6 → Erfolg: Die Tür öffnet sich ohne Alarm.



---

### 5) Glückspunkte (GP) — wann es sinnvoll ist, sie zu verwenden

Zu Beginn jeder Sitzung hast du **2 GP**. GP sind da, um:
 - wichtige Szenen zu retten,
 - Dramatik hinzuzufügen,
 - mutige Entscheidungen zu belohnen.

Gib **1 GP** aus, um eines zu wählen:
 - **Neuwurf** deines Tests (du behältst das bessere Ergebnis), oder
 - **Erhöhung des Würfels um 1 Stufe** für diesen einen Wurf, oder
 - **Umwandlung eines Misserfolgs in einen „Erfolg mit Kosten“** — die Aktion gelingt, aber der SL fügt sofort einen Preis hinzu.

**Rückgewinnung von GP:** Zu Beginn der nächsten Sitzung kehrst du auf das Limit zurück. Der SL kann **+1 GP** für mutiges Risiko, großartige erzählerische Entscheidungen oder das Spielen mit Konsequenzen verleihen.

**Beispiel:** Ein Misserfolg beim Sprung zwischen Dächern würde einen Sturz auf die Straße bedeuten. Du gibst 1 GP aus und verwandelst den Misserfolg in einen Erfolg mit Kosten: Du erreichst den anderen Dachrand, verlierst aber Ausrüstung oder verstauchst dir den Knöchel (schlechtere Ausgangslage in der nächsten Szene).

---



---

### 6.1 Entfernungen (standardmäßig, ohne Karte)

Beschreiben Sie die Entfernung mit vier Wörtern:
- **Nah** (in Reichweite),
- **Nicht weit** (einige Schritte),
- **Weit** (andere Seite der Szene),
- **Sehr weit** (scharfschützen- / fahrzeugmäßig).

In deinem Zug hast du: **Bewegung + 1 Aktion.**  
Bewegung ändert normalerweise die Entfernung um 1 Stufe (Nicht weit→Nah usw.).

### 6.2 Option: Spiel auf dem Gitter

Wenn ihr auf einer Karte spielt:
- 1 Kästchen = 1–2 m,
- Bewegung in der Runde: **bis zu 5 Kästchen**,
- Diagonalen zählen als 1 Kästchen,
- der Rest der Regeln funktioniert identisch.

### 6.3 Angriff

- **Nahkampf:** Wurf **<span class="rpg-token token-math">St</span>ärke (<span class="rpg-token token-stat">S</span>)** gegen die **Verteidigung** des Ziels.  
- **Fernkampf:** Wurf **Geschicklichkeit (<span class="rpg-token token-stat">Z</span>)** gegen die **Verteidigung** des Ziels.

**Verteidigung der Gegner (ungefähr):**
- <span class="rpg-token token-t">4</span> Schwach  
- <span class="rpg-token token-t">5</span> Gewöhnlich  
- <span class="rpg-token token-t">6</span> Elite  
- <span class="rpg-token token-t">8</span> Boss  
- <span class="rpg-token token-t">12</span> Legendärer Boss

### 6.4 Deckung und Position

- Ziel in Deckung / schlechter Winkel / Druck → schlechtere Situation (senke den Würfel).
- Gute Position / Überraschung / zahlenmäßiger Vorteil → bessere Situation (erhöhe den Würfel).

### 6.5 Treffer und Schaden

- Ein Treffer verursacht **1 Herz**.
- Ein außergewöhnlicher Erfolg verursacht **2 Herzen** oder hat einen starken Effekt (Entwaffnen, Umwerfen, Wegstoßen, aus der Deckung treiben).

### 6.6 0 Herzen

Wenn du auf **0 Herzen** fällst, bist du aus der Handlung ausgeschieden (verwundet, betäubt, unter Schock - gemäß den Konventionen). - Ein Verbündeter kann eine Aktion verwenden, um dich auf **1 Herz** zu bringen. - Wenn der Druck anhält, ist dein Vorrang der Schutz und die Evakuierung, nicht das „Tanking“. 

### Beispiel eines kurzen Zuges (ohne Gitter)

- Du bist **Nah** an der Elite.
- Bewegung: Du gehst **Nahe** hinter eine <span class="rpg-token token-stat">S</span>äule (Deckung).
- Aktion: Nahkampfangriff (<span class="rpg-token token-stat">S</span>). Die Verteidigung der Elite ist <span class="rpg-token token-t">6</span>. Du hast <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.  
  Wurf 9: Erfolg, die Elite verliert 1 Herz.




---

### 7) Kräfte und Spielzüge über dem Standard (Machtpunkte)

Das, was wir „Macht“ nennen, hängt von der Welt ab: Magie, Psionik, Glaube, Gadgets, Hacking, Supertricks.

### 7.1 Wie benutzt man die Macht

1) Beschreibe den Effekt.  
2) Der Spielleiter nennt den Schwierigkeitsgrad und die Kosten in <span class="rpg-token token-power">PM</span>.  
3) Gib <span class="rpg-token token-power">PM</span> aus und würfle mit **Macht (<span class="rpg-token token-stat">M</span>)**.

### 7.2 Effektstufen (T / Kosten)

- **Trick:** kurzer Effekt, Trick → <span class="rpg-token token-t">T 4</span>, Kosten 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Standard:** Angriff, Schild, Impuls → <span class="rpg-token token-t">T 5</span>, Kosten 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Stark:** Bereich, Heilung, Lähmung, „Live“-Hack → <span class="rpg-token token-t">T 6</span>, Kosten 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Großartig:** Szenenwechsel, mächtiger Eingriff → <span class="rpg-token token-t">T 8–12</span>, Kosten 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 Misserfolg und außergewöhnlicher Erfolg

- Misserfolg: die ausgegebenen <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span> gehen verloren, und die Konsequenz tritt ein (Überlastung, Spur, Verlust der Position, Nebenwirkung).
- Maximalwert auf dem Würfel: außergewöhnlicher Erfolg + zusätzlicher Vorteil (größere Reichweite, längere Dauer, <span class="rpg-token token-math">st</span>ärkerer Effekt oder weniger „Nebenwirkungen“).

### 7.4 <span class="rpg-token token-power">PM</span> Wiederherstellung

- Nach einer Konfliktszene erhältst du **1 <span class="rpg-token token-power">PM</span>** zurück. - Nach einer sicheren Pause – bis zur vollen Kapazität (sofern die Spielwelt dies zulässt).

**Beispiel (Fantasy):** „Kurzer Sprung“ – Standard, <span class="rpg-token token-t">T 5</span>, Kosten 1 <span class="rpg-token token-power">PM</span>.  
**Beispiel (Sci-Fi):** „Elektronisches Schloss überladen“ – Standard, <span class="rpg-token token-t">T 5</span>, Kosten 1 <span class="rpg-token token-power">PM</span>.



---

### 8) Ruhe und Erholung

Wenn ihr einen sicheren Moment habt (Zuflucht, Verband, Service, Mahlzeit):
- erholt ihr euch vollständig an **Herzen**,
- und füllt **MP** gemäß der Erholungsregel in eurer Konvention auf.

In strengeren Kampagnen kann der SL einen vollständigen Halt verlangen, um alles zurückzuerlangen.

---



---

### 9) Charakterentwicklung (wenn Du „levelst“)

Die Entwicklung erfolgt **nach dem Abenteuer** (in der Regel nach 1–3 Sitzungen, abhängig vom Tempo der Kampagne).
Wähle **eins**:
- Erhöhe ein Attribut um 1 Würfelstufe (max. bis <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>), oder
- +1 Herz (max. 7), oder
- +1 MP (max. 5), oder
- Neues Talent (eine kurze, einzeilige Regel, die mit dem SL vereinbart wird).

**Beispiel:** Geschicklichkeit steigt von <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> zu <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>. Von nun an machst Du alle Geschicklichkeitsproben mit <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.

---



---

### 10) Variante „nur <span class="rpg-token token-d6">k6</span>“: 2k6

Wenn ihr nur mit <span class="rpg-token token-d6">k6</span> spielen möchtet:

- Jeder Test ist **2k6 + Eigenschaftsmodifikator**.
- Anfangsmodifikatoren für Eigenschaften: eine Eigenschaft **+2**, eine **+1**, eine **+0**.

**Ergebnis:**
- **6 oder weniger** – Misserfolg mit Konsequenz  
- **7–9** – Erfolg mit Kosten  
- **10+** – voller Erfolg  
- **12** – außergewöhnlicher Erfolg

**Situation:** gib **+1 / -1** zum Wurf (begünstigt / behindert), anstatt die Schwellen zu ändern.

**Glück in 2k6:** funktioniert identisch, nur „Erhöhung der Würfel“ ersetzt durch **+1 zum Wurf**.



---

### 11) Gute Spielergewohnheiten

- Sprich: **was du tust + warum**. Das Ziel der Aktionen erleichtert es dem SL, den Einsatz festzulegen. - Wenn die Schwierigkeit hoch ist: nicht den „Wurf erzwingen“ — **ändere die Situation** (Vorbereitung, Werkzeug, Deckung, Hilfe, anderer Weg). - Zusammenarbeit: die Hilfe eines Verbündeten ist eine der <span class="rpg-token token-math">st</span>ärksten und einfachsten Hebel im System. - Im Kampf gewinnt die Position: Deckung, Distanz und situative Vorteile sind oft wichtiger als die Statistik.

