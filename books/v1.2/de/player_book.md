---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.2
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
generated_at: "2026-01-13T06:26:48.820Z"
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

### MG beschreibt die Situation und sagt, was möglich ist.
- Du sagst, **was du tust** und **welchen Effekt du möchtest**.
- Wenn das Ergebnis ungewiss ist, sagt MG.

- MG beschreibt die Situation und sagt, was möglich ist.
- Du sagst, **was du tust** und **welchen Effekt du möchtest**.
- Wenn das Ergebnis unsicher ist, sagt der MG:
  1) welche Eigenschaft du verwendest (S/Z/M),
  2) wie hoch die Schwierigkeit ist (<span class="rpg-token token-tn">TN</span>),
  3) was bei einem Misserfolg passieren kann.
- Du würfelst **einen Würfel** deiner Eigenschaft und schaust, ob das Ergebnis ≥ <span class="rpg-token token-tn">TN</span> ist.

### Die kürzeste Regel



---

### 1. Einleitung

Twoja postać ma:
- **Rolę** (Krieger / Schurke / Magier),
- 3 **Eigenschaften**: Stärke (S), Geschicklichkeit (G), Magie (M),
- **Leben** (Herzen) und **Mana**,
- 2 **Talente** (optional, aber empfohlen),
- Ausrüstung.

### 2.1 Eigenschaften (S/Z/M) — wozu są
- **Stärke (S)**: Nahkampf, Durchsetzen, Heben, Ausdauer.
- **Geschicklichkeit (Z)**: Schüsse, Präzision, Schleichen, Ausweichen, Akrobatik.
- **Magie (M)**: „spezielle” Effekte (Zauber/Psionik/Technologie — je nach Spiel).

### 2.2 Eigenschaftenwürfel
Jede Eigenschaft hat ihren eigenen Würfel (z.B. <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>). Du wirfst **immer** einen Würfel.
- Größerer Würfel = höhere Chance auf hohe Ergebnisse.

### 2.3 Leben und Mana
- **Leben:** 5 Herzen (Start).
- **Mana:** 3 (Start). Du gibst sie aus, wenn du Magie verwendest.



---

### Schritt 1: Wähle eine Rolle
Wähle eine Rolle. Legt die Startwürfel für die Eigenschaften fest:
- **Krieger:** S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- **Schurke:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- **Magier:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>

### Schritt 2: Ressourcen aufzeichnen

### Schritt 3: Wähle 2 Talente (optional)
Talente sind kurze Schlagworte, die beschreiben, worin du gut bist.
- Neutrale Beispiele: „Verhandler“, „Späher“, „Mechaniker“, „Sanitäter“, „Athlet“, „Analytiker“, „Hacker“.

**Wie Talente funktionieren:** Wenn ein Talent tatsächlich im Test hilft, kann der SL die **Schwierigkeit (<span class="rpg-token token-tn">TN</span>) um 1 Grad senken**.
- In der Regel 1 Talent pro Test.
- Ein Talent ersetzt nicht die Beschreibung der Handlung — es hilft, wenn es tatsächlich sinnvoll ist.

### Schritt 4: Ausrüstung
Liste auf:
- 1 Kampfinstrument (Nah- oder Fernkampf),
- Schutz (falls passend),
- 3 nützliche Gegenstände.

Ausrüstung in diesem Spiel funktioniert oft als **„Erlaubnis”**: Du hast etwas, also kannst du bestimmte Aktionen versuchen.

### Beispielcharakter
- Rolle: Schurke
- S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Leben 5, Mana 3
- Talente: „Späher”, „Verhandler”
- Ausrüstung: Fernkampfwaffe, Dietriche, Seil, Taschenlampe



---

### 4.1 Wann du würfelst
Du würfelst, wenn:
- etwas **riskant** oder ungewiss ist,
- und ein Misserfolg Konsequenzen hat.

Wenn etwas offensichtlich und ohne Druck ist, kann der Spielleiter sagen „es gelingt“ ohne zu würfeln.

### 4.2 Schwierigkeiten (<span class="rpg-token token-tn">TN</span>)
Es werden 4 Schwierigkeitsgrade verwendet:
- **<span class="rpg-token token-tn">TN</span> 4 — Einfach**
- **<span class="rpg-token token-tn">TN</span> 6 — Normal**
- **<span class="rpg-token token-tn">TN</span> 8 — Schwierig**
- **<span class="rpg-token token-tn">TN</span> 12 — Heldentat**

Der Spielleiter wählt die <span class="rpg-token token-tn">TN</span>. Du musst sie nicht „erraten“ — der Spielleiter sagt einfach, wie hoch die Schwierigkeit ist.

### Wyniki Testu

> **Schwierigkeitsgrad (<span class="rpg-token token-tn">TN</span>)**: 4 (Einfach), 6 (Normal), 8 (Schwierig).
> 
> **Wurf Ergebnis:**
> - **1**: Niederlage + Komplikation.
> - **< <span class="rpg-token token-tn">TN</span>**: Niederlage.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Erfolg.
> - **Max (10/20)**: Erfolg + Vorteil.

---

### 4.3 Würfelergebnisse
- **Ergebnis ≥ <span class="rpg-token token-tn">TN</span>:** Erfolg.
- **Ergebnis < <span class="rpg-token token-tn">TN</span>:** Misserfolg.
- **Wurf 1:** Misserfolg mit Komplikation.
- **Maximal auf den Würfeln** (z.B. 10 auf <span class="rpg-token token-d10">d10</span>): außergewöhnlicher Erfolg + zusätzlicher Vorteil.

**Zusätzlicher Vorteil** (Beispiele): schneller, leiser, sicherer, größerer Effekt, bessere Position.

### 4.4 Änderungen der Schwierigkeit „um einen Grad”
Anstatt Boni zu zählen, ändert der Spielleiter manchmal den Zielwert (ZV) um 1 Grad:
- schlechtere Bedingungen → ZV höher (z.B. 6 → 8),
- bessere Bedingungen → ZV niedriger (z.B. 8 → 6).

Deine Rolle als Spieler: **schaffe bessere Bedingungen** durch Beschreibung und Entscheidungen (Schutz, Vorbereitung, Werkzeuge, Plan).

### 4.5 Hilfe eines Verbündeten
Ein Verbündeter kann seine Aktion einsetzen, um dir zu helfen. Dann kannst du für diesen einen Wurf:
- den Würfel um 1 Größe erhöhen: **<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**.

Die Hilfe muss im Kontext sinnvoll sein (z. B. Deckung geben, Ablenkung schaffen, Werkzeuge übergeben).

### Beispieltest
Du möchtest schnell einen blockierten Durchgang öffnen.
- SL: „Das ist Geschicklichkeit, SW 6.”
- Du würfelst [token:<span class="rpg-token token-d10">d10</span>] und es fällt 7 → Erfolg: Durchgang geöffnet.



---

### 1 kurze

- **1 Feld** ist die grundlegende Einheit der Distanz.
- In einer Runde hast du **eine Bewegung von bis zu 5 Feldern**.
- Du kannst diagonal gehen (diagonal zählt als 1 Feld).
- Deckung ist wichtig: Wenn etwas dich vor einem Fernangriff schützt, ist es normalerweise schwieriger zu treffen.



---

### 6.1 Wie sieht eine Runde aus
In deiner Runde hast du:
- **Bewegung** (bis zu 5 Feldern),
- **1 Aktion**.

Eine Aktion kann z.B. sein: Angriff, Benutzung von Ausrüstung, Fähigkeitsprüfung, Hilfe, Einsatz von Magie.

### Atak

> 1) Wybierz cel (im Reichweite und in Sichtlinie).
> 2) Wybierz broń/czar.
> 3) Sprawdź, jakiej Cechy używa (z.B. Körperkraft, Geschicklichkeit auf Distanz, Magie für den Zauber).
> 4) **Würfle.** Vergleiche mit **<span class="rpg-token token-tn">TN</span>** des Gegners.

---

### 6.2 Angriff
- **Nahkampf:** Wurf auf **Stärke (S)**.
- **Distanz:** Wurf auf **Geschicklichkeit (G)**.
- Der Spielleiter nennt die Schwierigkeit des Gegners.

Standard-Schwierigkeiten der Gegner:
- **Wachposten:** Schwierigkeit 6
- **Elite:** Schwierigkeit 8
- **Boss:** Schwierigkeit 12

### Trafienie

> - **Pachołek**: Stirbt (oder scheidet aus dem Kampf aus).
> - **Elita/Boss**: Verliert **1 Herz**.
> - **Spieler**: Verliert **1 Herz** (es sei denn, er hat Rüstung — dann absorbiert die Rüstung den Treffer, wird aber verbraucht).

---

### 6.3 Was bedeutet ein Treffer
- Du triffst den Pylon → er scheidet aus dem Kampf aus.
- Du triffst die Elite/den Boss → er erhält eine Wunde (der Boss hat standardmäßig 3 Wunden).
- Außergewöhnlicher Erfolg gegen die Elite/den Boss → du fügst normalerweise +1 Wunde zu (insgesamt 2), oder du erhältst einen situativen Vorteil (z.B. das Herausdrängen aus der Deckung).

### Pudło i Odwet

> Walka ma ryzyko. Jeśli **nie trafisz** (wynik < <span class="rpg-token token-tn">TN</span>) lub wyrzucisz **1**:
> - Przeciwnik kontratakuje: tracisz **1 Serce**.
> - Albo dzieje się inna logiczna komplikacja (np. tracisz broń, zostajesz przewrócony).
> 
> *To nie jest tura przeciwnika — to efekt Twojego nieudanego ataku.*

---

### 6.4 Pudło und „Rache”
Wenn du **verfehlst** (Ergebnis < <span class="rpg-token token-tn">TN</span>) und der Gegner dich tatsächlich erreichen konnte, verlierst du **1 Herz**.
- Im Nahkampf ist das häufig.
- Bei Fernangriffen hängt viel von der Deckung und der Situation ab.

Deine taktische Lektion: **Positioniere dich so, dass du bei einem Fehlschuss keine Rache erhältst** (Deckung, Distanz, Plan, Hilfe).

### 0 Serc

> Wenn du auf 0 Herzen fällst:
> - Du bist **Niedergelegt**.
> - Du kannst keine Aktionen ausführen (nur kriechen und mit den letzten Kräften sprechen).
> - Ein Verbündeter kann dich „aufrichten“ (Aktion Hilfe), wodurch 1 Herz wiederhergestellt wird.
> - Wenn du Schaden erleidest, während du Niedergelegt bist — **stirbst du**.

---

### 6.5 0 Herzen
Wenn du auf 0 Herzen fällst:
- bist du umgekippt und führst keine Aktionen aus,
- kann ein Verbündeter eine Aktion verwenden, um dich mit **1 Herzen** wieder auf die Beine zu bringen.

### Beispiel für eine kurze Runde
- Bewegung: Du läufst 3 Felder zur Deckung.
- Aktion: Du schießt (Z). SL: „SW 6, aber das Ziel ist hinter Deckung → SW 8”. Du würfelst <span class="rpg-token token-d10">d10</span>=9 → Treffer.



---

### 1. Einleitung

Magie zur Mechanik „Spezialeffekte”. Du beschreibst den Effekt, der Spielleiter legt die Schwierigkeit und die Kosten für Mana fest.

### 7.1 Kosten und Stufen
- **Trick:** <span class="rpg-token token-tn">TN</span> 4, Kosten 0–1
- **Standard:** <span class="rpg-token token-tn">TN</span> 6, Kosten 1
- **Starker Effekt:** <span class="rpg-token token-tn">TN</span> 8, Kosten 2
- **Große Macht:** <span class="rpg-token token-tn">TN</span> 12, Kosten 3

### 7.2 Misserfolg in der Magie
Wenn die Magie misslingt:
- verlierst du die ausgegebene Mana,
- es tritt eine Konsequenz auf (z.B. −1 Herz, Verlust der Position, zusätzliche Bedrohung).

### 7.3 Außergewöhnlicher Erfolg
Ein maximaler Würfelwurf in der Magie bietet einen zusätzlichen Vorteil:
- größere Reichweite/Bereich,
- längere Dauer,
- höhere Effektivität,
- oder geringere Kosten (der Spielleiter kann 1 Mana zurückgeben).

### Beispiel Magie
Du möchtest einen kurzen „Sprung” von 5 Feldern machen.
- SL: „Das ist Standard: <span class="rpg-token token-tn">TN</span> 6, Kosten 1.”
- Du zahlst 1 Mana, würfelst M <span class="rpg-token token-d10">d10</span>=7 → Erfolg: Du springst hinter die Deckung.



---

### 1. Einleitung

Nach einem Konflikt, wenn ihr einen sicheren Moment und grundlegende Bedingungen für eine Ruhepause habt:
- Leben und Mana werden auf volle Werte zurückgesetzt.



---

### 1. Einleitung

Nach dem Abenteuer wählst du **eine**:
- Erhöhe S/Z/M um 1 Würfelgröße: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- oder +1 Herz (max 7),
- oder +1 Mana (max 5).

Das bedeutet Entwicklung, ohne weitere Würfel zu den Würfen hinzuzufügen.



---

### 1. Einleitung

Wenn auf dem Tisch nur ein <span class="rpg-token token-d6">d6</span> liegt, hast du anstelle der Würfelgröße die Erfolgsgrenze:
- Meister 3+, Geübt 4+, Novize 5+, Ohne Fertigkeit 6.

Der Spielleiter kann die Grenze um 1 Stufe anheben/senken, je nach Situation oder Unterstützung.



---

### Immer sprechen

- Sag immer: **was du tust** + **warum**. „Ich möchte den Hebel drücken” ist okay, aber „ich möchte den Hebel drücken, um den Durchgang zu schließen” ist noch besser.
- Wenn <span class="rpg-token token-tn">TN</span> hoch ist: nicht „Wurf quälen” — ändere die Situation (Deckung, Werkzeuge, Hilfe, anderer Weg).
- Vereinbart die Zusammenarbeit: eine Person hilft, die andere führt den Test durch.
- In einem Kampf respektiere die Deckung und Position — oft ist sie wichtiger als der Wurf selbst.

---
Ende des Spielerhandbuchs.

