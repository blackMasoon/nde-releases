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
generated_at: "2026-01-14T12:06:46.307Z"
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
# Start (Rules in a Nutshell)



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

### 2) How to resolve actions

1. Choose the relevant attribute (S/D/M) and roll that die.
2. Compare to the Target Number (<span class="rpg-token token-tn">TN</span>):
   - Easy 4, Standard 6, Hard 8, Heroic 12.
3. Result:
   - Rolling a 1 — failure with a complication (noise, time loss, minor harm, etc.).
   - Result < <span class="rpg-token token-tn">TN</span> — failure.
   - Result ≥ <span class="rpg-token token-tn">TN</span> — success.
   - Maximum on the die (e.g., 10 on <span class="rpg-token token-d10">d10</span>, 20 on <span class="rpg-token token-d20">d20</span>) — critical success with an extra benefit.
Quality without math:
- Worse/better situation: move <span class="rpg-token token-tn">TN</span> up/down by 1 step (e.g., 6 → 8 due to cover).
- Ally Help (uses their action): for this roll, bump your die up one size (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
Example: Warrior kicks a door (<span class="rpg-token token-tn">TN</span> 6). Rolls <span class="rpg-token token-d10">d10</span>=10 — critical: the door bursts and a minion behind is knocked over.




---

### 3) Grid movement and combat

- Movement: up to 5 squares (diagonals allowed).
- Your turn: Move + 1 Action (e.g., attack, spell, search, pull lever).
- Attack:
  - Melee (S): roll vs the foe’s <span class="rpg-token token-tn">TN</span>.
  - Ranged (D): target in cover raises <span class="rpg-token token-tn">TN</span> by 1 step.
- Foes’ TNs: Minion 6, Elite 8, Boss 12.
- On a hit: Minion — removed; Elite — GM may require favorable conditions; Boss — has 3 Wounds (each hit = 1 Wound). Critical vs Boss = 2 Wounds.
- Retaliation: if you miss in melee or within realistic reach, you lose 1 Heart (unless in full cover).
Example: Mage (D <span class="rpg-token token-d6">d6</span>) slings a stone at a minion behind a crate: <span class="rpg-token token-tn">TN</span> 6 + cover → 8. Mage asks Rogue to Help (die to <span class="rpg-token token-d8">d8</span>) and takes a better position (<span class="rpg-token token-tn">TN</span> back to 6). <span class="rpg-token token-d8">d8</span>=7 — hit.




---

### 4) Magic

- Casting: describe effect, spend Mana, roll Magic (M).
  - Trick (spark, noise, fog) — <span class="rpg-token token-tn">TN</span> 4, cost 0–1 Mana.
  - Bolt/Shield/Short Blink (5 squares) — <span class="rpg-token token-tn">TN</span> 6, cost 1 Mana.
  - Area/Heal +2 Hearts/Paralyze — <span class="rpg-token token-tn">TN</span> 8, cost 2 Mana.
  - Great power (bridge of ice, storm of fire) — <span class="rpg-token token-tn">TN</span> 12, cost 3 Mana.
- Failure: Mana is spent; add a small consequence (breathless −1 Heart or unwanted attention).
- After a fight: you recover all Mana; a safe rest also restores Hearts.
Example: “Blink” (short teleport 5 squares): <span class="rpg-token token-tn">TN</span> 6, cost 1 Mana. Mage <span class="rpg-token token-d10">d10</span> rolls 7 — success behind cover.



---

### 5) Down and healing

- At 0 Hearts: you are down (no actions). An ally can use an Action to bring you to 1 Heart.
- After a clash, with a brief safe rest and supplies, everyone returns to full Hearts and Mana.
Example: Rogue drops to 0. Warrior helps — Rogue returns at 1 Heart.




---

### 6) Advancement (no extra dice on the table)

After an adventure choose one:
- Raise one attribute’s die size: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- or +1 Heart (max 7),
- or +1 Mana (max 5).
Example: Warrior raises Strength from <span class="rpg-token token-d10">d10</span> to <span class="rpg-token token-d12">d12</span> — hitting <span class="rpg-token token-tn">TN</span> 12 gets easier.




---

### 7) <span class="rpg-token token-d6">d6</span>‑only variant

If you only have a single <span class="rpg-token token-d6">d6</span>:
- Replace die sizes with success thresholds per attribute:
  - Master 3+, Trained 4+, Novice 5+, Untrained 6.
- <span class="rpg-token token-tn">TN</span> still shifts situation by 1 step (easier/harder).
- Help: lower the threshold by 1 (e.g., 4+ → 3+ for this roll).
- Advancement: raise one attribute’s level (e.g., Trained 4+ → Master 3+) or +1 Heart/Mana.
Example: Rogue (Trained 4+) shoots at a lightly covered target (one step harder) → needs 5+. <span class="rpg-token token-d6">d6</span>=5 — hit.


