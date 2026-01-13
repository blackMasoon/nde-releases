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
generated_at: "2026-01-13T06:26:30.156Z"
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
# Core Rules



---



---

- A squared grid (paper, battle mat, or VTT) and tokens/miniatures.
- Pencil and a character sheet.
- Dice: <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>.
  - Practically, one of each per table is enough — you roll a single die at a time.
  - If you only have <span class="rpg-token token-d6">d6</span>, use the <span class="rpg-token token-d6">d6</span>‑only variant at the end.




---

These appear throughout the rules — here they are in plain language:

- GM (Game Master): describes the situation, controls the world and opposition, sets Target Numbers (<span class="rpg-token token-tn">TN</span>) and consequences.
- Player: declares what the character does and rolls the die.
- Square: one cell on the grid; used to measure distance and movement.
- Move: moving a character a number of squares.
- Action: one meaningful thing in your turn (attack, ability, trigger a mechanism, cast, etc.).
- Turn: your opportunity to Move and take one Action.
- Test: a die roll that resolves uncertainty.
- <span class="rpg-token token-tn">TN</span> (Target Number): the number you must meet or beat to succeed.
- Attributes: Strength (S), Dexterity (D), Magic (M). Each has a die size.
- Attribute die: the die size tied to an attribute (e.g., D <span class="rpg-token token-d10">d10</span>).
- Success: result ≥ <span class="rpg-token token-tn">TN</span>.
- Critical success: the maximum value on the die (e.g., 12 on <span class="rpg-token token-d12">d12</span>). Grants an extra benefit in addition to success.
- Complication: an extra problem on failure — noise, time loss, dropped gear, worse position, spent resource.
- Cover: an obstacle between attacker and target; usually increases <span class="rpg-token token-tn">TN</span> for ranged attacks.
- Retaliation: consequence of missing in combat — you lose 1 Heart if the foe could effectively strike back.
- Heart: a hit point in the simplest sense.
- Mana: resource used for Magic (could represent tech/psionics in other genres).
- Wound (Boss/Elite): a hit that reduces a tougher foe. Bosses fall after several Wounds.




---

Character creation is intentionally brief: pick a role, assign three attribute dice, note resources.


### 2.1 Roles (pick one)
- Warrior — specializes in Strength (melee, force).
- Rogue — specializes in Dexterity (shots, stealth, precision, evasion).
- Mage — specializes in Magic (special effects, control, power).

Role names are technical. In another setting they can mean soldier/agent/specialist.


### 2.2 Attributes and dice
You have three attributes:
- Strength (S) — force, endurance.
- Dexterity (D) — speed, finesse, stealth.
- Magic (M) — special effects: spells, psionics, tech, superhuman ability (setting‑dependent).

Each attribute has a die size. At start:
- Warrior: S <span class="rpg-token token-d10">d10</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- Rogue:   S <span class="rpg-token token-d6">d6</span>,  D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Mage:    S <span class="rpg-token token-d6">d6</span>,  D <span class="rpg-token token-d6">d6</span>,  M <span class="rpg-token token-d10">d10</span>


### 2.3 Resources
- Hearts: 5.
- Mana: 3.


### 2.4 Talents (optional but recommended)
Talents are two short keywords that describe what your character is notably good at (still setting‑neutral):
- e.g., Negotiator, Mechanic, Scout, Analyst, Athlete, Medic, Hacker.

How Talents work: if a Talent genuinely helps on a test, the GM may lower the <span class="rpg-token token-tn">TN</span> by one step.
- Talents don’t grant automatic success.
- Usually at most one Talent applies to a single test.


### 2.5 Gear
Write down:
- a weapon or combat tool,
- protection (optional),
- three useful items for the adventure.

Gear in the core rules acts as permission (it enables actions) rather than numeric bonuses.


### 2.6 Sample character
- Role: Rogue
- Attributes: S <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Hearts: 5, Mana: 3
- Talents: Scout, Negotiator
- Gear: ranged tool, lockpicks, rope, light source




---

If you understand this section, you understand the system.


### 3.1 When to roll
Roll only when both are true:
1) the outcome is uncertain, and
2) failure changes something or has a cost.

If a task is trivial and pressure‑free, the GM can just say “it works”.


### 3.2 How to perform a test (step by step)
1) The player states **what they are doing** and **what effect they want**.
2) The GM chooses a characteristic: S, Z, or M.
3) The GM sets the **<span class="rpg-token token-tn">TN</span>** (Difficulty) and any situational modifiers.
4) The player rolls **one characteristic die**.
5) Compare the result to the <span class="rpg-token token-tn">TN</span> and determine the outcomes.

### 3.3 Difficulty scale (<span class="rpg-token token-tn">TN</span>)
Use four bands:
- <span class="rpg-token token-tn">TN</span> 4 (Easy): likely if competent or conditions favor you.
- <span class="rpg-token token-tn">TN</span> 6 (Standard): default difficulty.
- <span class="rpg-token token-tn">TN</span> 8 (Hard): needs advantage, prep, or specialization.
- <span class="rpg-token token-tn">TN</span> 12 (Heroic): significant challenge; often requires <span class="rpg-token token-d12">d12</span>/<span class="rpg-token token-d20">d20</span>, great setup, or both.


### Wyniki Testu

> **Target Number (<span class="rpg-token token-tn">TN</span>)**: 4 (Easy), 6 (Normal), 8 (Hard).
> 
> **Roll Result:**
> - **1**: Failure + Complication.
> - **< <span class="rpg-token token-tn">TN</span>**: Failure.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Success.
> - **Max (10/20)**: Success + Benefit.

---

### 3.4 Outcomes
- Result ≥ <span class="rpg-token token-tn">TN</span> → Success.
- Result < <span class="rpg-token token-tn">TN</span> → Failure.
- Rolling a 1 → Failure + Complication (even if <span class="rpg-token token-tn">TN</span> is low).
- Max on the die → Critical success (success plus an extra benefit appropriate to the fiction).


### 3.5 Adjusting difficulty without math
Instead of adding/subtracting numbers, shift <span class="rpg-token token-tn">TN</span> by one step.

- Worse conditions → <span class="rpg-token token-tn">TN</span> +1 step (e.g., cover, darkness, slick surface, time pressure, noise, distractions).
- Better conditions → <span class="rpg-token token-tn">TN</span> −1 step (e.g., prep, proper tools, superior position, surprise, full focus).

For extremes, you may shift by two steps.

Bounds:
- If <span class="rpg-token token-tn">TN</span> would fall below 4, treat it as “almost certain” (often no roll).
- If <span class="rpg-token token-tn">TN</span> would exceed 12, treat it as “nearly impossible” (requires a new plan/approach).


### 3.6 Help from an ally
An ally can spend their Action (or time outside combat) to assist.

Effect: bump the roller’s die up one size for that single test:
- <span class="rpg-token token-d6">d6</span> → <span class="rpg-token token-d8">d8</span> → <span class="rpg-token token-d10">d10</span> → <span class="rpg-token token-d12">d12</span> → <span class="rpg-token token-d20">d20</span>

Order rules:
- Usually only one helper per test (avoid “help towers”).
- The help must make sense in fiction: covering fire, handing tools, distracting, steadying, giving instructions.


### 3.7 Re‑rolling
Don’t repeat the same test over and over without a change.
- Change approach (different attribute/tools/route), or
- accept a complication (time, alarm), or
- withdraw.


### 3.8 Examples (non‑combat)
Example A — quiet crossing:
- Player: “I want to cross an open area unseen.”
- GM: Dexterity. It’s dusk with some cover → <span class="rpg-token token-tn">TN</span> 6.
- Roll <span class="rpg-token token-d10">d10</span>=5 → failure. GM: “You’re not spotted yet, but someone heard a sound and starts checking (complication: time pressure).”

Example B — tools and force:
- Player: “I want to get the mechanism working fast.”
- GM: Strength if it’s brute force, Magic if it’s a special interface; here it’s Strength. <span class="rpg-token token-tn">TN</span> 6.
- Ally helps (bump to <span class="rpg-token token-d12">d12</span>). Roll <span class="rpg-token token-d12">d12</span>=12 → critical: it works instantly and silently.




---

How we measure on the board.


### 4.1 Squares
- 1 square = base unit of distance.
- Diagonals are allowed and count as 1.


### 4.2 Movement
- Default movement: up to 5 squares on your turn.
- You may move before or after your Action (or split movement).


### 4.3 Line and cover (simple)
- Full cover: target is completely blocked → cannot be hit by ranged attacks.
- Partial cover: target is visible but protected → ranged <span class="rpg-token token-tn">TN</span> +1 step.

Apply cover to perception/stealth tests as fits the fiction.




---

Combat is a normal scene with turns.


### 5.1 When combat starts
When at least one side tries to harm the other and timing matters.

If it would be trivial/obvious, resolve with a single test.


### 5.2 Turn order (simple)
- All players act (any order), then
- all foes act, repeat.

This keeps pace fast. For more tactical play, add initiative (see GM book).


### 5.3 What you can do on your turn
On your turn, you have:
- **Movement** (up to 5 squares),
- **1 Action**.

An action can be:
- an attack,
- a skill check (e.g., pulling a lever, running through a hazard),
- using equipment,
- assisting an ally,
- using Magic.

### Atak

> Translation pending...

---

### 5.4 Attacking
1) Pick a target (in reach and line).
2) Pick attack type:
   - Melee → Strength test,
   - Ranged → Dexterity test.
3) Set the target’s <span class="rpg-token token-tn">TN</span>.
4) Roll.

Foes’ <span class="rpg-token token-tn">TN</span> (core):
- Minion: 6
- Elite: 8
- Boss: 12


### Trafienie

> Translation pending...

---

### 5.5 On a hit
- Minion: removed from the fight.
- Elite: takes 1 Wound; standard Elite has 2 Wounds.
- Boss: takes 1 Wound; Boss has 3 Wounds.
- Critical success: vs Elite/Boss either +1 Wound (total 2) or another sensible boon (push, disarm, seize position) — choose one.

You can simplify by using only Minions and Bosses.


### Pudło i Odwet

> Translation pending...

---

### 5.6 Misses and retaliation
If result < <span class="rpg-token token-tn">TN</span> and the foe could realistically hit back, the attacker loses 1 Heart.

“Could hit back” guidelines:
- In melee (adjacent) — usually yes.
- At range in the open with a responsive foe — often yes.
- Behind full cover or beyond practical reach — usually no.

Rolling a 1 in combat: failure + complication (e.g., lose 1 Heart and get knocked prone, drop gear, or get pushed from cover).


### 5.7 Ranges (defaults)
- Melee: adjacent.
- Ranged: any visible target.
  - If you want a limit: treat up to 10 squares as no penalty; beyond that <span class="rpg-token token-tn">TN</span> +1 step.


### 5.8 Multiple foes in close
If many minions are adjacent to one hero, either:
- raise <span class="rpg-token token-tn">TN</span> by 1 step (pressure), or
- have failure include an extra complication (lose position).

Keep it fast: one resolution → one outcome.


### 5.9 Combat examples
Example A — simple melee exchange:
- Warrior (S <span class="rpg-token token-d10">d10</span>) adjacent to a minion (<span class="rpg-token token-tn">TN</span> 6).
- Roll <span class="rpg-token token-d10">d10</span>=4 → miss; retaliation triggers → Warrior loses 1 Heart.

Example B — boss and critical:
- Rogue (D <span class="rpg-token token-d10">d10</span>) shoots a Boss (<span class="rpg-token token-tn">TN</span> 12). GM: “Hard without setup.”
- Ally helps (die to <span class="rpg-token token-d12">d12</span>) and Rogue gains position (<span class="rpg-token token-tn">TN</span> 12 → 8).
- Roll <span class="rpg-token token-d12">d12</span>=12 → critical: Boss takes 2 Wounds.




---

“Magic” is the umbrella for special effects; in other genres it can be psionics or tech.


### 6.1 Mana
- Start with 3 Mana.
- Spend Mana when attempting effects beyond normal capability.


### 6.2 How to adjudicate
1) Describe the effect.
2) GM sets <span class="rpg-token token-tn">TN</span> and Mana cost.
3) Spend Mana.
4) Roll Magic (M) vs <span class="rpg-token token-tn">TN</span>.

Failure: effect fizzles; Mana is spent; add a small consequence.


### 6.3 Effect tiers (<span class="rpg-token token-tn">TN</span> and cost)
- Trick — <span class="rpg-token token-tn">TN</span> 4, cost 0–1: light, sound, smoke, brief distraction.
- Standard — <span class="rpg-token token-tn">TN</span> 6, cost 1: bolt, barrier, 5‑square blink, short buff.
- Strong — <span class="rpg-token token-tn">TN</span> 8, cost 2: area, control, heal +2 Hearts, immobilize.
- Great power — <span class="rpg-token token-tn">TN</span> 12, cost 3: large scene‑changing effect.


### 6.4 Critical magic
On a max roll with Magic:
- increase scale (area/duration/potency), or
- reduce cost (GM may refund 1 Mana), or
- add another benefit (quiet, precise, safe for allies).


### 6.5 Magic examples
Example A — defensive run:
- Player: “I set a quick barrier to sprint 5 squares safely.”
- GM: Standard <span class="rpg-token token-tn">TN</span> 6, cost 1. Roll M <span class="rpg-token token-d10">d10</span>=9 → success.

Example B — failure and fallout:
- Player: “I try to pin an elite” (<span class="rpg-token token-tn">TN</span> 8, cost 2).
- Roll 3 → failure: effect fizzles, spend 2 Mana, plus a complication (exposed).




---

### 7.1 Hearts (life)
- By default, you have **5 Hearts**.
- Losing a Heart means real damage or exhaustion — depending on the world.

### 0 Serc

> Translation pending...

---

### 7.2 0 Hearts
If you fall to 0 Hearts:
- you are **down** and cannot take actions,
- an ally can spend an Action to get you back on your feet with **1 Heart**.

### 7.3 Rest
After a scene of combat/conflict, if you have a moment of safe rest (and basic conditions), you return to full:
- Hearts,
- Mana.

This keeps the system fast and does not require lengthy healing.



---

After an adventure (or major milestone) choose one:
- bump S/D/M die size (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>),
- or +1 Heart (max 7),
- or +1 Mana (max 5).

Note: a bigger die means more effectiveness without adding more dice to the table.




---

If you prefer a single <span class="rpg-token token-d6">d6</span>:


### 9.1 Thresholds instead of die sizes
Each attribute has a <span class="rpg-token token-d6">d6</span> target:
- Master: 3+
- Trained: 4+
- Novice: 5+
- Untrained: 6


### 9.2 Situational difficulty
Shift the threshold one step for harder/easier situations (min 2+, max 6).


### 9.3 Help
Help lowers the threshold by 1 for that roll.


### 9.4 Combat mapping
- Minion: Standard (no change).
- Elite: Hard (+1 to threshold).
- Boss: Heroic (+2) and 3 Wounds.


### 9.5 Advancement
Raise one attribute’s level (e.g., Novice→Trained) or +1 Heart/Mana.




---

1) What exactly is the player trying to achieve?
2) Which attribute applies: S/D/M?
3) What’s the <span class="rpg-token token-tn">TN</span> (4/6/8/12), and does the situation shift it by a step?
4) Any help (bump die)?
5) Roll → success/failure.
6) On failure: which complication (or retaliation in combat)?
7) On critical: which extra benefit?




---

### 1. Introduction

7.2 Additional tools are not required, but they can sometimes facilitate management.

### 11.1 Protection (armor) as a simple resource
- A character with protection has 1 Armor token per scene.
- When they would lose 1 Heart (retaliation/hit), they may spend Armor instead.


### 11.2 Time pressure as a clock
- If a scene is time‑sensitive, set a “clock” (e.g., 3‑step). Each failure advances it by 1. When it fills, the bad outcome triggers (alarm, target escapes, passage collapses).

---
End of the Basic Rules Book.


