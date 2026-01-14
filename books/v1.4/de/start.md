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
generated_at: "2026-01-14T12:06:46.372Z"
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
# Regeln auf einen Blick

Automatic translation placeholder for de

---



---

### [ERROR] 1) Bohater w 1 minutę

[Translation Failed] * **Koncept:** kim jesteś i w jakim gatunku grasz (1 zdanie).
* **Rola (wybierz jedną):**

  * **Szturm** – presja, walka, przełamywanie przeszkód
  * **Specjalista** – skradanie, precyzja, technika, obserwacja
  * **Adept** – moce, wiedza, wpływ, improwizacja
* **Cechy (3):**

  * **Siła (S)** – siła fizyczna, wytrzymałość, walka wręcz
  * **Zręczność (Z)** – refleks, skradanie, strzelanie, pilotowanie
  * **Moc (M)** – magia/psionika/technologia/blef/intuicja (zależnie od świata)
* **Kości cech:** jedna cecha **<span class="rpg-token token-d12">k12</span>**, jedna **<span class="rpg-token token-d8">k8</span>**, jedna **<span class="rpg-token token-d6">k6</span>** (wybierz zgodnie z rolą).
* **Serca:** 5. **Punkty Mocy:** 3 (wydajesz na moce i „zagrania specjalne”).
Poniżej masz gotowy fragment do wklejenia (wariant A), w stylistyce krótkich zasad „1-page”.

**Łut Szczęścia (jak działa):** wydaj **1 ŁS**, aby wybrać jedno:

* **Przerzut** swojego testu (zostawiasz lepszy wynik), albo
* **Podbicie kości o 1 stopień** na ten jeden rzut (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), albo
* **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę (np. tracisz czas, robisz hałas, zużywasz zasób, kończysz w gorszej pozycji, przyciągasz uwagę, psujesz sprzęt).

**Odzysk ŁS:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 ŁS** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

* **Ekwipunek:** 1 narzędzie „kluczowe” (np. miecz, karabin, zestaw hakerski), 1 ochrona (pancerz, tarcza energetyczna, kamuflaż), 3 drobiazgi pasujące do konceptu.

**Przykład:** Specjalista: Z <span class="rpg-token token-d12">k12</span>, M <span class="rpg-token token-d8">k8</span>, S <span class="rpg-token token-d6">k6</span>. W cyberpunku M to „Hacking/Influence”; w fantasy M to „Magia/Wola”.



---

### 2) Wie führst du Aktionen aus

1. Wähle die passende Eigenschaft (S/Z/M) und würfle mit dem Würfel dieser Eigenschaft.
2. Vergleiche mit dem Schwierigkeitsgrad (<span class="rpg-token token-tn">TN</span>):
   - Einfach 4, Normal 6, Schwer 8, Heldisch 12.
3. Ergebnis:
   - 1 auf dem Würfel — Misserfolg mit Komplikation (Lärm, Zeitverlust, kleine Verletzung usw.).
   - Ergebnis < <span class="rpg-token token-tn">TN</span> — Misserfolg.
   - Ergebnis ≥ <span class="rpg-token token-tn">TN</span> — Erfolg.
   - Maximal auf dem Würfel (z.B. 10 auf <span class="rpg-token token-d10">d10</span>, 20 auf <span class="rpg-token token-d20">d20</span>) — außergewöhnlicher Erfolg mit zusätzlichem Vorteil.
Verbesserungen ohne Zählung:
- Bessere/ schlechtere Situation: senke/ erhöhe <span class="rpg-token token-tn">TN</span> um 1 Stufe (z.B. 6 → 8 durch Deckung).
- Hilfe eines Verbündeten (mit seiner Aktion): für diesen Wurf „steigere“ den Würfel um eine Größe (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
Beispiel: Der Krieger rammt die Tür auf (Normal 6). Er würfelt <span class="rpg-token token-d10">d10</span> und erzielt 10 — außergewöhnlicher Erfolg: die Tür fliegt auf, und der Wache dahinter fällt um.



---

### 3) Bewegung und Kampf auf dem Spielfeld

- Bewegung: bis zu 5 Felder (Diagonalen erlaubt).
- Dein Zug: Bewegung + 1 Aktion (z. B. Angriff, Zauber, Durchsuchen, Hebel ziehen).
- Angriff:
  - Nahkampf (N): Wurf gegen die <span class="rpg-token token-tn">TN</span> des Gegners.
  - Fernkampf (F): Deckung des Ziels erhöht die <span class="rpg-token token-tn">TN</span> um 1 Stufe.
- <span class="rpg-token token-tn">TN</span> der Gegner: Fußsoldat 6, Elite 8, Boss 12.
- Auswirkungen eines Treffers: Fußsoldat — fällt nach einem Treffer; Elite — der SL kann günstige Bedingungen verlangen; Boss — hat 3 Wunden (Treffer = 1 Wunde). Außergewöhnlicher Erfolg gegen den Boss = 2 Wunden.
- Vergeltung: Wenn du im Nahkampf oder im Bereich der Vergeltung verfehlst, verlierst du 1 Herz (es sei denn, du hast vollen Schutz).
Beispiel: Magier (F <span class="rpg-token token-d6">d6</span>) schießt mit einer Schleuder auf den Fußsoldaten hinter der Kiste: <span class="rpg-token token-tn">TN</span> 6 + Deckung → 8. Der Magier bittet den Schurken um Hilfe (er erhöht den Würfel auf <span class="rpg-token token-d8">d8</span>) und wechselt die Position auf eine bessere (<span class="rpg-token token-tn">TN</span> sinkt auf 6). <span class="rpg-token token-d8">d8</span>=7 — getroffen.



---

### 4) Magie

- Zauber wirken: Beschreibe den Effekt, gib Mana aus, wirf Magie (M).
  - Trick (Flamme, Knall, Nebel) — SW 4, Kosten 0–1 Mana.
  - Geschoss/Schutz/Sprung 5 Felder — SW 6, Kosten 1 Mana.
  - Bereich/Heilung +2 Herzen/Paralyse — SW 8, Kosten 2 Mana.
  - Große Macht (Eisbrücke, Feuersturm) — SW 12, Kosten 3 Mana.
- Misserfolg: Mana geht verloren; es kommt zu einer kleinen Konsequenz (Kurzatmigkeit −1 Herz oder unerwünschte Aufmerksamkeit von Feinden).
- Ruhe nach dem Kampf: Du stellst alle Mana wieder her; ein sicherer Rast stellt auch Herzen wieder her.
Beispiel: „Blitz“ (kurze Teleportation 5 Felder): SW 6, Kosten 1 Mana. Magier <span class="rpg-token token-d10">d10</span> würfelt 7 — erfolgreicher Sprung hinter den Schutz.



---

### 5) Fall und Behandlung

- 0 Herzen: umgekippt (du bist handlungsunfähig). Ein Verbündeter kann eine Aktion verwenden, um dich auf 1 Herz zu heben.
- Nach dem Kampf, bei einer kurzen Pause und einer Mahlzeit, kehrt ihr zu vollen Herzen und Mana zurück.  
Beispiel: Der Schurke fällt auf 0. Der Krieger hilft ihm aufzustehen — der Schurke kehrt auf 1 Herz zurück.



---

### 6) Entwicklung der CHARAKTERE

Nach dem Abenteuer wähle eines:
- Erhöhe einen Attribut um die Größe des Würfels: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- oder +1 Herz (max 7),
- oder +1 Mana (max 5).
Beispiel: Der Krieger erhöht seine Stärke von <span class="rpg-token token-d10">d10</span> auf <span class="rpg-token token-d12">d12</span> — es ist einfacher, <span class="rpg-token token-tn">TN</span> 12 zu treffen.



---

### 7) Variante nur-<span class="rpg-token token-d6">d6</span>

Wenn ihr nur einen <span class="rpg-token token-d6">d6</span>-Wurf habt:
- Anstelle von Würfelgrößen hat jede Eigenschaft eine Erfolgsgrenze:
  - Meister 3+, Geübt 4+, Anfänger 5+, Ohne Fertigkeit 6.
- Die <span class="rpg-token token-tn">TN</span> verändert weiterhin die Situation um 1 Grad (leichter/schwerer).
- Hilfe: Senke die Grenze um 1 (z.B. von 4+ auf 3+ für diesen Wurf).
- Entwicklung: Erhöhe das Niveau einer Eigenschaft (z.B. Geübt 4+ → Meister 3+) oder +1 Herz/Mana.
Beispiel: Schuss des Schurken (Geübt 4+) auf ein Ziel in leichter Deckung (um einen Grad schwieriger) erfordert 5+. Wurf <span class="rpg-token token-d6">d6</span>=5 — Treffer.

