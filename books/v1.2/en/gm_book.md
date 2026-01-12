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
generated_at: "2026-01-12T10:14:46.184Z"
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
# Game Master Book



---



---

- State stakes clearly. Before the roll: attribute, <span class="rpg-token token-tn">TN</span>, failure consequence, and whether help is possible.
- Fiction → mechanics → result. Always start from the fiction, then call for a roll.
- Keep scenes snappy. One test = one meaningful effect.
- Failure moves the situation forward. Complications change the fiction rather than resetting it.
- Consistency. Same circumstances → same <span class="rpg-token token-tn">TN</span> and effects.




---

1) Player states intent and approach.
2) Pick attribute: S (force), D (speed/precision), M (special effect).
3) Set <span class="rpg-token token-tn">TN</span>: 4 easy, 6 standard, 8 hard, 12 heroic.
4) Announce failure stakes and whether someone can help (bump die by one size).
5) Player rolls and compares to <span class="rpg-token token-tn">TN</span>.
6) Apply outcome and update the situation.

Table shorthand: “Attr/<span class="rpg-token token-tn">TN</span>/Roll/Effect”.




---

- 4 (easy): favorable conditions, no active opposition.
- 6 (standard): default in adventures without advantage.
- 8 (hard): time pressure, bad position, cover, complex tools.
- 12 (heroic): above‑average challenge; often needs preparation or a big die.

Situational adjustment: shift <span class="rpg-token token-tn">TN</span> by one step (max two for extremes).
- Worse: dark, slick, cover, alarm → <span class="rpg-token token-tn">TN</span> +1.
- Better: time, tools, high ground, surprise → <span class="rpg-token token-tn">TN</span> −1.

Quick odds intuition (rough):
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17%; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38%; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50%; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58%.
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30%; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42%; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45%.
Use as guidance only; don’t math at the table.

When not to roll:
- If the outcome is obvious and there’s no stake.
- If rolling won’t change anything — move on.




---

- 1 on the die: failure + complication. Examples: noise, time loss, bad lead, minor harm (−1 Heart), spent resource, worse position.
- Failure (result < <span class="rpg-token token-tn">TN</span>): no effect plus potential retaliation in combat, or threat progress outside combat.
- Critical (max on die): success + extra benefit (faster/quieter/no cost/bigger effect).

Complication checklist:
1) Hit a resource (time, position, hearts, mana, gear).
2) Change the map (new obstacle, blocked route, improved enemy cover).
3) Raise pressure (clock, alarm, reinforcements).




---

- Movement: up to 5 squares; diagonals allowed.
- Cover: partial → ranged <span class="rpg-token token-tn">TN</span> +1; full → no line.
- Difficult terrain (optional): entering a cell costs 2 of 5 movement.
- Shove/push: S vs <span class="rpg-token token-tn">TN</span> 6 (adjust by fiction). Success: move target 1–2 squares; critical: +1 square.
- Ranges: treat up to 10 squares as no penalty; further → <span class="rpg-token token-tn">TN</span> +1.
Prioritize speed over minutiae.




---

- Order: players → opponents → repeat.
- Attacks: melee = S, ranged = D; foe TNs: minion 6, elite 8, boss 12.
- Hits: minion off the board; elite/boss +1 Wound (boss has 3). Criticals usually = 2 Wounds.
- Miss: if foe could strike back → attacker loses 1 Heart (retaliation). From full cover/far away → usually no retaliation.

Scaling pressure:
- Several minions in close → <span class="rpg-token token-tn">TN</span> +1 or add a complication on a miss.
- Evolve terrain each round: obstacles, chokepoints, opportunities for advantage.




---

Do it in 5 steps:
1) Goal: why the scene exists (cross/secure/disable/steal/escort/defend).
2) Obstacles: 2–3 different types (guards, lock, alarm, hazardous area).
3) Threat: minions/elites/boss, hazards, traps.
4) Clock (optional): 3–5 steps; failures tick it; at max, the bad outcome triggers.
5) Reward/Consequence: what success grants; how failure changes things.

Encounter sizing for 3–5 PCs (guidelines):
- Easy: 3–5 minions or a lone elite.
- Standard: 6–8 minions or 1 elite + 2–4 minions.
- Hard: boss + 2–4 minions or 2 elites + 3–5 minions.
- Heroic: boss + 4–6 minions and/or an elite.
Adjust for terrain and cover — they matter a lot.




---

Format (setting‑neutral):
> Name — <span class="rpg-token token-tn">TN</span>, Wounds, Role, Special
- Minion: <span class="rpg-token token-tn">TN</span> 6, no Wounds; simple tactics.
- Elite: <span class="rpg-token token-tn">TN</span> 8, 2 Wounds; has a clear edge (mobility, cover, control).
- Boss: <span class="rpg-token token-tn">TN</span> 12, 3 Wounds; 1–2 unique moves (push, summon, barrier, etc.).

Reaction/morale (lightweight):
- When the first minion falls or an elite is wounded, roll <span class="rpg-token token-d6">d6</span>:
  - 1–2: withdraw/hunker; 3–4: hold; 5–6: press.
- Modify ±1 for advantage/fear/boss nearby.




---

Assign <span class="rpg-token token-tn">TN</span> and Mana cost per tier:
- Trick: <span class="rpg-token token-tn">TN</span> 4, 0–1 (small, quick effect).
- Standard: <span class="rpg-token token-tn">TN</span> 6, 1 (single target, short blink, barrier).
- Strong: <span class="rpg-token token-tn">TN</span> 8, 2 (area, control, heal +2 Hearts).
- Great power: <span class="rpg-token token-tn">TN</span> 12, 3 (scene‑changer).

Helpers:
- Multiple targets: either +1 Mana or <span class="rpg-token token-tn">TN</span> +1 step.
- Sustained effect: pay 1 Mana per round or it occupies the caster’s Action.
- Countering/evading: allow a relevant PC test (D or M) vs the same <span class="rpg-token token-tn">TN</span> to reduce/avoid the effect if fictionally justified.




---

- Stealth/assassination: set an Alarm clock (3–5). Failures tick it; at max, patrol arrives/locks engage.
- Chase: track distance in “chase steps” (e.g., 3). Each round both sides roll; pursuer success shrinks, runner success grows. At 0 → caught; at 5 → escape.
- Environmental obstacles: state the cost clearly (fall = −1 Heart and worse position). <span class="rpg-token token-tn">TN</span> depends on fiction.




---

- Advancement: after an adventure each PC picks one — bump a die size, +1 Heart (max 7) or +1 Mana (max 5).
- Material rewards: grant permissions (new actions) or one‑shot boons (“once per scene lower a <span class="rpg-token token-tn">TN</span> by 1”). Avoid permanent numeric modifiers.
- Economy (optional): coarse tiers (cheap/standard/expensive). Resolve with a resource test instead of counting currency.




---

- Agree on boundaries and lines/veils up front.
- Provide a simple “pause/rewind” signal for uncomfortable content.
- Resolve disagreements in fiction, not at the table.




---

1) Hook: one‑sentence problem.
2) 3 locations with tactical features (cover, height, narrow passages).
3) 3 obstacles: lock, patrol, environmental threat.
4) Stakes: time, noise, attention.
5) Complication list (5) and a clock.
6) Opponents: one‑line entries (minions/elites/boss) + simple tactics.




---

Complications — <span class="rpg-token token-d6">d6</span> (universal):
1. Time loss / enemy advantage.
2. Position revealed / alarm rises.
3. Minor harm: −1 Heart or resource.
4. Bad position: pushed/stuck.
5. Gear lost/jammed.
6. A new threat enters the scene.

Critical benefits — <span class="rpg-token token-d6">d6</span>:
1. Faster.
2. Quieter.
3. No cost (no Mana/retaliation).
4. Bigger effect (area/range).
5. Better ally position.
6. Extra clue/information.




---

- Goal: cross a secured passage.
- GM preps: lock (<span class="rpg-token token-tn">TN</span> 6), patrol (clock 3), narrow corridor (cover).
1) Player A: “I pick the lock” (D, <span class="rpg-token token-tn">TN</span> 6). Failure ticks clock. Roll 5 → fail, clock 1/3.
2) Player B helps (bump die). A tries again with new tools/better position, rolls <span class="rpg-token token-d12">d12</span>=9 → success.
3) Patrol nears (clock 2/3). Player C covers the exit (S, <span class="rpg-token token-tn">TN</span> 6). Critical grants a strong position for the team.
Fast resolution, transparent stakes.

---
That’s all you need to run. The rest (setting, monster lists, treasures) is modular and should fit your chosen genre.


