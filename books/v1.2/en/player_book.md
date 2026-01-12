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
generated_at: "2026-01-12T10:14:57.848Z"
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
# Player Book



---



---

- The GM describes the situation and options.
- You say what you do and what result you want.
- If the outcome is uncertain, the GM tells you:
  1) which attribute you use (S/D/M),
  2) the difficulty (<span class="rpg-token token-tn">TN</span>),
  3) what happens on failure.
- You roll a single attribute die and check if result ≥ <span class="rpg-token token-tn">TN</span>.


### The shortest rule
Roll your attribute die. Result ≥ <span class="rpg-token token-tn">TN</span> = success.




---

You have:
- a Role (Warrior / Rogue / Mage),
- 3 Attributes: Strength (S), Dexterity (D), Magic (M),
- Hearts (life) and Mana,
- 2 Talents (optional but recommended),
- gear.


### 2.1 What the attributes do
- Strength (S): melee, forcing, lifting, endurance.
- Dexterity (D): shots, precision, stealth, dodging, acrobatics.
- Magic (M): special effects (spells/psionics/tech — setting dependent).


### 2.2 Attribute dice
Each attribute has a die (<span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>). You always roll one die.
- Bigger die = better odds of high results.


### 2.3 Hearts and Mana
- Hearts: 5 (start).
- Mana: 3 (start). Spend it when using Magic.




---

### Step 1: Pick a role
This sets your starting dice:
- Warrior: S <span class="rpg-token token-d10">d10</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- Rogue:   S <span class="rpg-token token-d6">d6</span>,  D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Mage:    S <span class="rpg-token token-d6">d6</span>,  D <span class="rpg-token token-d6">d6</span>,  M <span class="rpg-token token-d10">d10</span>


### Step 2: Note resources
- Hearts: 5
- Mana: 3


### Step 3: Pick 2 Talents (optional)
Short keywords that describe strengths.
- Neutral examples: Negotiator, Scout, Mechanic, Medic, Athlete, Analyst, Hacker.

How Talents work: if a Talent truly helps, the GM may lower <span class="rpg-token token-tn">TN</span> by one step.
- Usually 1 Talent per test.
- Talent doesn’t replace description — it helps when it actually applies.


### Step 4: Gear
List:
- one combat tool (melee or ranged),
- protection (if appropriate),
- 3 utility items.

Gear mostly acts as permission: you have it, so you can try certain things.


### Example character
- Role: Rogue
- S <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Hearts 5, Mana 3
- Talents: Scout, Negotiator
- Gear: ranged tool, lockpicks, rope, light source




---

### 4.1 When you roll
You roll when it’s risky/uncertain and failure matters.

If it’s obvious and pressure‑free, GM can say “it works”.


### 4.2 Difficulty (<span class="rpg-token token-tn">TN</span>)
Four bands:
- <span class="rpg-token token-tn">TN</span> 4 — Easy
- <span class="rpg-token token-tn">TN</span> 6 — Standard
- <span class="rpg-token token-tn">TN</span> 8 — Hard
- <span class="rpg-token token-tn">TN</span> 12 — Heroic

The GM sets <span class="rpg-token token-tn">TN</span>. No need to guess — the GM tells you.


### Wyniki Testu

> **Target Number (<span class="rpg-token token-tn">TN</span>)**: 4 (Easy), 6 (Normal), 8 (Hard).
> 
> **Roll Result:**
> - **1**: Failure + Complication.
> - **< <span class="rpg-token token-tn">TN</span>**: Failure.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Success.
> - **Max (10/20)**: Success + Benefit.

---

### 4.3 Outcomes
- Result ≥ <span class="rpg-token token-tn">TN</span>: success.
- Result < <span class="rpg-token token-tn">TN</span>: failure.
- Roll a 1: failure with a complication.
- Max on the die (e.g., 10 on <span class="rpg-token token-d10">d10</span>): critical success + extra benefit.

Extra benefit examples: faster, quieter, safer, bigger effect, better position.


### 4.4 Shifting difficulty by a step
Instead of math, the GM shifts <span class="rpg-token token-tn">TN</span> by one step:
- worse conditions → <span class="rpg-token token-tn">TN</span> up (e.g., 6 → 8),
- better conditions → <span class="rpg-token token-tn">TN</span> down (e.g., 8 → 6).

Your job: create better conditions via description (cover, prep, tools, plan).


### 4.5 Help from an ally
An ally can spend their Action to help. For that roll you may bump your die:
- <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>.

The help must make sense (covering, distraction, handing tools).


### Test example
You try to open a blocked passage quickly.
- GM: “Dexterity, <span class="rpg-token token-tn">TN</span> 6.”
- You roll D <span class="rpg-token token-d10">d10</span> = 7 → success: passage opens.




---

- 1 square is the basic unit of distance.
- Movement per turn: up to 5 squares.
- Diagonals count as 1.
- Cover matters: ranged attacks into cover are harder.




---

### 6.1 Your turn
- Move up to 5 squares and take 1 Action.

Actions include: attack, use gear, attribute test, help, use Magic.


### Atak

> Translation pending...

---

### 6.2 Attacks
- Melee: Strength roll.
- Ranged: Dexterity roll.
- The GM states the foe’s <span class="rpg-token token-tn">TN</span>.

Default foe <span class="rpg-token token-tn">TN</span>:
- Minion: 6
- Elite: 8
- Boss: 12


### Trafienie

> Translation pending...

---

### 6.3 What a hit means
- Minion → out of the fight.
- Elite/Boss → takes a Wound (Boss has 3 total).
- Critical vs Elite/Boss → usually +1 Wound (total 2) or one positional boon (push, eject from cover).


### Pudło i Odwet

> Translation pending...

---

### 6.4 Misses and retaliation
If you miss (result < <span class="rpg-token token-tn">TN</span>) and the foe could hit back, you lose 1 Heart.
- Common in melee.
- At range it depends on cover/position.

Tactical lesson: position yourself to avoid retaliation on a miss (cover, distance, plan, help).


### 0 Serc

> Translation pending...

---

### 6.5 At 0 Hearts
- You’re down and can’t act.
- An ally can spend an Action to bring you to 1 Heart.


### Short turn example
- Move: dash 3 squares to cover.
- Action: shoot (D). GM: “<span class="rpg-token token-tn">TN</span> 6, but target has cover → <span class="rpg-token token-tn">TN</span> 8.” You roll <span class="rpg-token token-d10">d10</span>=9 → hit.




---

Magic is the “special effects” mechanic. You describe the effect; the GM sets <span class="rpg-token token-tn">TN</span> and Mana cost.


### 7.1 Costs and tiers
- Trick: <span class="rpg-token token-tn">TN</span> 4, cost 0–1
- Standard: <span class="rpg-token token-tn">TN</span> 6, cost 1
- Strong: <span class="rpg-token token-tn">TN</span> 8, cost 2
- Great power: <span class="rpg-token token-tn">TN</span> 12, cost 3


### 7.2 Failure in Magic
If it fails:
- you lose the Mana spent, and
- a consequence appears (e.g., −1 Heart, exposed, extra threat).


### 7.3 Critical magic
Max roll with Magic grants an extra boon:
- bigger area/range,
- longer duration,
- higher potency,
- or reduced cost (GM may refund 1 Mana).


### Magic example
You try a short 5‑square “blink”.
- GM: “Standard: <span class="rpg-token token-tn">TN</span> 6, cost 1.”
- You pay 1 Mana, roll M <span class="rpg-token token-d10">d10</span>=7 → success behind cover.




---

After a conflict, if you have a safe moment and basic rest conditions:
- Hearts and Mana return to full.




---

After an adventure choose one:
- bump S/D/M die size: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- or +1 Heart (max 7),
- or +1 Mana (max 5).




---

If you only have a <span class="rpg-token token-d6">d6</span>, replace die sizes with thresholds:
- Master 3+, Trained 4+, Novice 5+, Untrained 6.

The GM may raise/lower your threshold by one step for situation or help.




---

- Always say what you do and why. Intent helps the GM pick clear stakes.
- If <span class="rpg-token token-tn">TN</span> is high, don’t brute‑force the roll — change the situation (cover, tools, help, new route).
- Coordinate: one helps, the other rolls.
- In combat, cover and position often matter more than the roll.

---
End of the Player’s Book.


