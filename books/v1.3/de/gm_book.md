---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.3
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
generated_at: "2026-01-13T12:23:01.314Z"
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
# Spielleiterhandbuch

Automatic translation placeholder for de

---



---

### 7.2. Klare Kommunikation des Satzes.

- **Kommuniziere die Schwierigkeit klar.** Bevor der Wurf erfolgt, sage: Eigenschaft, Zielwert, Konsequenz des Scheiterns, Chance auf Hilfe.
- **Beschreibung → Mechanik → Ergebnis.** Beginne immer mit der Fiktion, dann erst der Wurf.
- **Schnelle Szenen.** Halte das Tempo: ein Test = ein sinnvoller Effekt.
- **Scheitern treibt die Aktion voran.** Eine Komplikation verändert die Situation und „setzt“ die Szene nicht zurück.
- **Kohärenz.** Die gleichen Umstände → die gleichen Zielwerte und Konsequenzen.



---

### 1. Einleitung

1) Der Spieler sagt, was er tut und was er erreichen möchte.  
2) Wähle eine Eigenschaft: **S** (stark), **Z** (präzise/schnell), **M** (spezielle Effekte).  
3) Bestimme **<span class="rpg-token token-tn">TN</span>**: 4 leicht, 6 normal, 8 schwierig, 12 heldenhaft.  
4) Sage, was bei einem Misserfolg droht und ob jemand **helfen** kann (Wurf um 1 Größe erhöhen).  
5) Der Spieler würfelt mit der Eigenschaft und vergleicht mit der <span class="rpg-token token-tn">TN</span>.  
6) Entscheide über das Ergebnis und aktualisiere die Situation.  

Abkürzung für den Tisch: „Eigenschaften/<span class="rpg-token token-tn">TN</span>/Wurf/Folge“.



---

### 4 (einfach):

- **4 (einfach):** die Bedingungen sind günstig, das Ziel leistet keinen Widerstand.
- **6 (normal):** Standard in einem Abenteuer ohne Vorteil.
- **8 (schwierig):** Zeitdruck, schlechte Position, Deckung, komplexe Werkzeuge.
- **12 (heldenhaft):** überdurchschnittliche Herausforderung; erfordert normalerweise Vorbereitung oder hohe Würfel.

Situative Modifikation: verschiebe die <span class="rpg-token token-tn">TN</span> **um 1 Stufe** (max. um 2 in Extremfällen).
- Schlechter: dunkel, rutschig, Deckung, Alarm → <span class="rpg-token token-tn">TN</span> +1.
- Besser: Zeit, Werkzeuge, Positionsvorteil, Überraschung → <span class="rpg-token token-tn">TN</span> −1.

Schnelle Intuitionen zur Effektivität (Annäherungen):
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17%; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38%; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50%; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58%.
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30%; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42%; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45%.
Verwende diese Zahlen als Orientierung, rechne nicht ständig nach.

Wann nicht würfeln:
- Wenn das Ergebnis offensichtlich ist und es keinen Einsatz gibt.
- Wenn der Wurf nichts ändern würde (besser, zur nächsten Herausforderung überzugehen).



---

### 1 auf den Würfeln

- **1 auf den Würfeln**: Misserfolg + Komplikation. Beispiele: Lärm, Zeitverlust, falsche Fährte, kleine Wunde (−1 Herz), verlorene Ressource, schlechtere Position.
- **Misserfolg (Ergebnis < <span class="rpg-token token-tn">TN</span>)**: kein Effekt und eventuell „Rache“ (im Kampf) oder Fortschritt der Bedrohung (außerhalb des Kampfes).
- **Außergewöhnlicher Erfolg (maximal auf den Würfeln)**: Erfolg + zusätzlicher Vorteil: schneller/leichter/ohne Kosten/größerer Effekt.

Checkliste zur Erstellung von Komplikationen:
1) Greife eine Ressource an (Zeit, Position, Herzen, Mana, Ausrüstung).
2) Ändere das Layout auf dem Spielfeld (neue Hindernisse, abgeschnittene Wege, verstärkte Deckungen).
3) Erhöhe den Druck (Zähler, Alarm, Verstärkung der Gegner).



---

### Bewegung:

- **Bewegung:** bis zu 5 Felder (Reichweite 5) oder 1 Zone.
- **Rennen:** Wenn du nicht angreifst, kannst du dich 2x so weit bewegen (10 Felder / 2 Zonen).



---

### Reihenfolge:

- **Reihenfolge:** Spieler → Gegner → wiederholen.
- **Angriff:** Nahkampf = S, Fernkampf = Z; <span class="rpg-token token-tn">TN</span> des Gegners: Handlanger 6, Elite 8, Boss 12.
- **Treffer:** Handlanger fällt; Elite/Boss erhält 1 Wunde (Boss hat 3). Außergewöhnlicher Erfolg = normalerweise 2 Wunden.
- **Fehlschuss:** wenn der Gegner erreichen konnte → Held verliert 1 Herz (Rache). In Deckung/weit weg — normalerweise keine Rache.

Skalierung des Drucks:
- Viele Handlanger „im Nahkampf“ → <span class="rpg-token token-tn">TN</span> +1 oder zusätzliche Komplikation bei Fehlschuss.
- Ändere das Terrain jede Runde: Hindernisse, Engpässe, Gelegenheiten für Vorteile erscheinen.



---

### 1. Einleitung

Bau Szenen in 5 Schritten:
1) **Ziel**: Wozu dient die Szene (z.B. Übergang, Beschaffung von Gegenständen, Ausschaltung einer Bedrohung).
2) **Hindernisse**: 2–3 verschiedene Typen (Wachen, Schloss, Alarm, gefährliches Terrain).
3) **Bedrohung**: Handlanger/Elite/Boss, Gefahren, Fallen.
4) **Zähler (optional)**: 3–5 Schritte; Misserfolge verschieben ihn; am Ende gibt es eine negative Konsequenz.
5) **Belohnung/Konsequenz**: Was bringt der Erfolg, was ändert sich bei einem Misserfolg.

Konfliktgrößen (für 3–5 Helden):
- **Einfach:** 3–5 Handlanger oder Elite ohne Unterstützung.
- **Standard:** 6–8 Handlanger oder Elite + 2–4 Handlanger.
- **Schwierig:** Boss + 2–4 Handlanger oder 2 Eliten + 3–5 Handlanger.
- **Heroisch:** Boss + 4–6 Handlanger und/oder Elite.
Anpassen an den Tisch: Terrain und Deckungen haben großen Einfluss.



---

### 1. Einleitung

Format (Beispiel, ohne Atmosphäre):
> **Name — <span class="rpg-token token-tn">TN</span>, Wunden, Taktik, Spezial**
- **Handlanger:** <span class="rpg-token token-tn">TN</span> 6, keine Wunden; einfache Taktik.
- **Elite:** <span class="rpg-token token-tn">TN</span> 8, 2 Wunden; hat einen klaren Vorteil (z.B. Mobilität, Deckung, Kontrolle des Feldes).
- **Boss:** <span class="rpg-token token-tn">TN</span> 12, 3 Wunden; 1–2 einzigartige Bewegungen (z.B. Wegstoßen, Unterstützung herbeirufen).

Reaktion und Moral (leichtes System):
- Wenn der erste Handlanger fällt oder die Elite eine Wunde erleidet, würfle **<span class="rpg-token token-d6">d6</span>**:
  - 1–2: Rückzug/Verstecken; 3–4: halten die Position; 5–6: greifen an.
- Modifiziere ±1 für Vorteil/Angst/Boss in der Nähe.



---

### 1. Einleitung

Magie sind „Spezialeffekte”. Weisen Sie <span class="rpg-token token-tn">TN</span> und Kosten für Mana gemäß der Skala zu:
- **Trick:** <span class="rpg-token token-tn">TN</span> 4, Kosten 0–1 (kurzer, kleiner Effekt).
- **Standard:** <span class="rpg-token token-tn">TN</span> 6, Kosten 1 (einzelnes Ziel, kurzer Sprung, Barriere).
- **Stark:** <span class="rpg-token token-tn">TN</span> 8, Kosten 2 (Bereich, Kontrolle, Heilung +2 Herzen).
- **Große Macht:** <span class="rpg-token token-tn">TN</span> 12, Kosten 3 (Bühneneffekt).

Hilfsregeln:
- **Mehrere Ziele:** entweder +1 Kosten für Mana oder <span class="rpg-token token-tn">TN</span> +1 Grad.
- **Aufrechterhaltung des Effekts:** jede Runde 1 Mana zahlen oder es kostet eine Aktion.
- **Gegenschlag/Zauber vermeiden:** erlauben Sie dem Helden, einen entsprechenden Test (Z oder M) gegen dasselbe <span class="rpg-token token-tn">TN</span> durchzuführen, um den Effekt zu reduzieren oder zu vermeiden (je nach Fiktion).



---

### Skrytobójstwo/przemykanie:** setze „Alarmstufe” auf **Zähler 3–5

- **Skrytobójstwo/przemykanie:** setze den „Alarmstufe” auf **Zähler 3–5**; Misserfolge erhöhen ihn; nach Erreichen des Maximums erscheint eine Patrouille, das Schloss wird verriegelt usw.
- **Verfolgung:** lege die Distanz in „Verfolgungsschritten” fest (z. B. 3). Jede Runde: beide Seiten testen; Erfolg des Verfolgers verkürzt, Erfolg des Entkommens verlängert. Wenn es auf 0 kommt → eingeholt; bei 5 → entkommen.
- **Umwelt-Hindernisse:** kommuniziere klar die Kosten des Risikos (z. B. Fall = −1 Herz und schlechtere Position), die <span class="rpg-token token-tn">TN</span> hängt von den Beschreibungen ab.



---

### Entwicklung:

- **Entwicklung:** Nach dem Abenteuer wählt jeder eines: Erhöhung der Eigenschaftswürfelgröße, +1 Herz (max 7) oder +1 Mana (max 5).
- **Sachbelohnungen:** Gewähren „Erlaubnisse“ (neue Aktionen) oder einmalige Vorteile („einmal pro Szene <span class="rpg-token token-tn">TN</span> um 1 senken“). Vermeide permanente Modifikatoren.
- **Ökonomie (optional):** Einfache Schwellenwerte: billig/standard/teuer — entscheide durch einen Ressourcen-Test, anstatt Währung zu zählen.



---

### 1. Einleitung

- Legen Sie mit den Spielern den Inhaltsspielraum fest (was ist in Ordnung, was vermeiden wir).
- Vereinbaren Sie ein einfaches Signal „Stopp”/„Vorwärts” für unangenehme Situationen.
- Konflikte sollten in der Fiktion ausgetragen werden, nicht am Tisch.



---

### 1. Einleitung

1) **Hak:** ein einzeiliger Konflikt.
2) **3 Orte** mit taktischen Merkmalen (Deckungen, Höhen, enge Durchgänge).
3) **3 Hindernisse:** Schloss, Wache, Umweltgefahr.
4) **Ressourcen im Spiel:** Zeit, Lärm, Aufmerksamkeit des Gegners.
5) **Liste der Komplikationen** (5 Stück) und **Zähler** für die Szene.
6) **Gegner:** einzeilige Einträge (Puppen/Elite/Boss) + einfache Taktik.



---

### 1. Einleitung

Komplikationen — <span class="rpg-token token-d6">d6</span> (universell):
1. Zeitverlust / Vorteil des Gegners.
2. Offenlegung der Position / Anstieg der Alarmbereitschaft.
3. Geringer Schaden: −1 Herz oder Ressource.
4. Schlechte Position: Herausgedrängt/Steckenbleiben.
5. Verlust/Einklemmen von Ausrüstung.
6. Neue Bedrohung erscheint in der Szene.

Vorteile bei außergewöhnlichem Erfolg — <span class="rpg-token token-d6">d6</span>:
1. Schneller.
2. Leiser.
3. Ohne Kosten (z.B. ohne Mana/ohne Vergeltung).
4. Größerer Effekt (Bereich/Reichweite).
5. Bessere Position der Verbündeten.
6. Zusätzlicher Hinweis/Information.



---

### Ziel der Spieler

- Ziel der Spieler: durch den gesicherten Durchgang gelangen.
- SL: Schloss (SG 6), Patrouille (Zähler 3), schmaler Durchgang (Deckungen).
1) Spieler A: „Ich öffne das Schloss“ (Wurf, SG 6). Misserfolg = +1 zum Zähler. Wurf 5 → Misserfolg, Zähler 1/3.
2) Spieler B hilft (würfelt mit einem zusätzlichen Würfel). A: erneut (neue Werkzeuge, bessere Position), Wurf <span class="rpg-token token-d12">d12</span>=9 → Erfolg.
3) Patrouille nähert sich (Zähler 2/3). Spieler C sichert den Ausgang (Wurf, SG 6). Außergewöhnlicher Erfolg → Vorteil für die Gruppe.
Szene schnell entschieden, mit klaren Einsätzen.

---
Das ist alles, was du für das Leiten benötigst. Der Rest (Welt, Monster, Schätze) ist modular und sollte an das gewählte Universum angepasst werden.

